# Guia do criador — do zero à primeira venda

## Público
Iniciantes, desenvolvedores, freelancers e pequenas empresas. O guia evoluirá junto com os recursos reais do VYRO.

## Etapa 1 — Conhecer o editor existente
1. Instale dependências e execute `npm run dev`.
2. Crie uma tela no canvas, adicione componentes e altere propriedades.
3. Teste o preview e a navegação oferecidos pelo editor original.
4. Salve e reabra um projeto.
5. Verifique as opções atuais de exportação. Não confunda prompt para IA com código executável.

## Etapa 2 — Planejar um sistema comercial
Exemplo: cadastro de clientes.
- Entidade Cliente: id UUID, nome obrigatório, e-mail opcional, telefone, data de criação.
- Telas: lista, formulário, detalhes.
- Ações: incluir, alterar, excluir com confirmação, pesquisar.
- Regras: validar nome, evitar exclusão acidental, registrar erros.
- Dados: banco persistente, migrações, backup.

## Etapa 3 — Implementar com o futuro App Builder
**Planejado, ainda indisponível:** criar entidade no editor, associar formulário, gerar API, executar migrações e exportar o aplicativo. Até essa fase ser entregue, essas operações requerem programação convencional.

## Etapa 4 — Testar antes de entregar
- Testar campos vazios e inválidos.
- Testar autenticação e permissões entre usuários.
- Verificar persistência após reinicialização.
- Conferir backup/restauração e logs.
- Testar em celular e desktop.
- Auditar dependências e licenças.

## Etapa 5 — Vender e manter
Defina escopo, entregáveis, prazo, propriedade intelectual, implantação, hospedagem, suporte, manutenção, atualizações e tratamento de dados em contrato. Não prometa funcionalidades ainda inexistentes.

## Exercícios
1. Desenhe um formulário de clientes com três campos.
2. Descreva cinco validações necessárias.
3. Faça um mapa de telas: listagem -> cadastro -> detalhes.
4. Escreva três testes para a operação de exclusão.
5. Liste custos mensais de um cliente hospedado.

## Créditos
VYRO App Builder — contribuições VYRO: Walney Moreira Klein — walneyk@hotmail.com. Base derivada de M3E Canvas; manter `LICENSE` e `NOTICE`.
