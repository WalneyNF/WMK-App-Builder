# Arquitetura proposta e segurança

## Base existente
- `app/Editor.tsx`: editor visual.
- `components/`: componentes da interface.
- `lib/i18n.ts`: traduções e idioma atual.
- `lib/ai.ts`: integrações iniciais de IA, atualmente com configurações armazenadas no navegador.
- `lib/project.ts`: modelo de projeto existente.

## Arquitetura futura — não implementada
```text
Editor visual -> Modelo declarativo versionado -> Validadores
                      |                         |
                      v                         v
               Motor de workflows        Geradores de código
                      |                         |
               API / banco de dados     HTML/React/servidor
                      |
               Agentes via orquestrador
                      |
               Logs + aprovação + testes
```

## Regras essenciais
- Modelo de projeto com versão de esquema, IDs estáveis, migrações e validação.
- Geração determinística para o mesmo projeto e versão de gerador.
- Separação entre editor, runtime, backend e projetos exportados.
- Aplicação exportada deve funcionar sem depender do editor.
- Agentes propõem mudanças em diffs; usuário aprova antes de gravar ou executar ações sensíveis.
- Ferramentas MCP e processos externos com permissões mínimas, escopo de arquivos, logs e limites de tempo.

## Segurança
`lib/ai.ts` usa `localStorage` para configurações que incluem chaves de API. Não usar esse desenho para uma oferta comercial multiusuário. Planejar backend autenticado, armazenamento seguro de segredos, controle de permissões e limites de consumo.

Impedir que código gerado ou agentes acessem livremente segredos, sistema de arquivos e banco de produção. Testar injeção, XSS, CSRF, autorização, SQL injection, dependências e proteção de dados. CORS não substitui autenticação.

## Compatibilidade
Não modificar o formato original de projeto sem testes de importação/exportação e migração. Manter o laboratório de agentes independente até a integração ter contrato e testes.
