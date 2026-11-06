# VYRO App Builder — Comece aqui

**Projeto:** VYRO App Builder — fork de M3E Canvas  
**Responsável pelas contribuições VYRO:** Walney Moreira Klein — walneyk@hotmail.com  
**Estado:** base original clonada; funcionalidades de app builder completo ainda planejadas.

## Visão
Criar um construtor visual open source de aplicativos web, com exportação de código, fluxos, banco de dados e integração supervisionada com agentes de IA. A ferramenta será aberta; aplicações desenvolvidas por terceiros poderão ser privadas e comerciais, conforme as licenças dos componentes utilizados.

## O que existe hoje
- Editor visual de telas Material 3 Expressive.
- Projeto Next.js, React e TypeScript.
- Internacionalização em japonês, inglês, chinês e coreano em `lib/i18n.ts`.
- Recursos iniciais de assistência de IA em `lib/ai.ts`.
- Testes automatizados em Vitest.

## O que NÃO está pronto
- Português brasileiro completo; gerador de aplicações full stack; CRUD visual com banco; hospedagem/publicação; orquestração dos agentes próprios; MCP completo.
- Não anunciar esses recursos como disponíveis até implementação e teste.

## Instalação de desenvolvimento
Requisitos: Node.js compatível com `package.json` e npm. No Windows:
```powershell
cd D:\VYRO-App-Builder
npm ci
npm run dev
```
Abrir o endereço local indicado pelo Next.js (geralmente http://localhost:3000). Para validar:
```powershell
npm run typecheck
npm test
npm run build
```
Os comandos são instruções; sua execução bem-sucedida precisa ser verificada no ambiente.

## Índice
1. `01-LICENCA-E-NEGOCIOS.md` — direitos, venda de apps e modelo comercial.
2. `02-ARQUITETURA-E-SEGURANCA.md` — módulos, limites e segurança.
3. `03-ROADMAP-E-CRITERIOS.md` — fases e critérios de aceitação.
4. `04-GUIA-DO-CRIADOR.md` — do primeiro protótipo à entrega comercial.

## Regra editorial
Todo manual deve distinguir **implementado**, **em desenvolvimento** e **planejado**. Incluir exemplos reproduzíveis, pré-requisitos, testes e riscos. Preservar licença, NOTICE e atribuições originais.
