# Roadmap com critérios de aceitação

## 0.1 — Base e identidade
- Criar branch de trabalho.
- Aplicar identidade VYRO sem remover atribuições legais.
- Adicionar `pt-BR` ao seletor e às estruturas de tradução.
- Preservar idiomas existentes.
- Executar typecheck, testes e build.
**Aceite:** alternância de idioma, edição, salvar/abrir e exportações existentes funcionando.

## 0.2 — Exportador de frontend
- Definir contrato JSON versionado.
- Gerar HTML/CSS/JS e React.
- Testes de snapshot e projeto de exemplo.
**Aceite:** projeto exportado executa independentemente do editor.

## 0.3 — CRUD comercial
- Entidades, formulários, validações, listagem e pesquisa.
- Backend de referência com SQLite e migrações.
- Testes de criação, leitura, edição, exclusão e persistência.
**Aceite:** cadastro de clientes funciona após reiniciar o servidor.

## 0.4 — Agentes
- Contrato de tarefas com orquestrador, agentes e provedores.
- Logs, cancelamento, timeouts, revisão de diff e aprovação.
- Suporte local por provedor compatível quando tecnicamente viável.
**Aceite:** agente modifica projeto de teste somente após aprovação.

## 0.5 — Workflows e publicação
- Ações visuais, autenticação e controle de acesso.
- Exportação com configuração por ambiente.
- Guia de implantação e rollback.
**Aceite:** aplicação publicada com backups e testes de segurança.

## 1.0 — Produto utilizável
- Documentação completa, templates, testes de regressão e licenças.
- Demonstração de aplicativo comercial real.
- Métricas de confiabilidade e suporte.
**Aceite:** desenvolvedor novo reproduz o tutorial de ponta a ponta.

## Política de qualidade
Não chamar mock de integração real. Não declarar fase concluída sem testes e evidências. Registrar bugs conhecidos e mudanças incompatíveis.
