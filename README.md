# Painel de Compras

Painel de acompanhamento de fornecedores, pedidos e programação de entregas.
Arquivo único, sem dependência externa — abre offline.

**Acesso:** https://iorran-moonventures.github.io/painel-compras/

## O que o painel mostra

- **Entregas** — calendário de recebimentos, com contorno verde para o que chegou e vermelho para o que venceu sem chegar
- **Fornecedores** — dashboard por fornecedor: quantidade, valor, evolução por mês, produtos e pedidos
- **Produtos** — visão por SKU, com os pedidos de cada item
- **Curva ABC** — prioridade de consumo, por valor e por quantidade
- **Condições de pagamento** — evolução do prazo médio ponderado

## Sobre os dados

Os números são um **retrato**, não dado ao vivo: a data da última atualização
aparece no canto superior direito. A publicação é diária.

Os nomes de fornecedor foram substituídos por códigos (`Fornecedor A`,
`Fornecedor B`, ...) e os números de pedido por sequência (`PED-0001`).
Preço unitário e informação de negociação de prazo não são publicados.

## Como é gerado

O painel é montado a partir de um banco SQLite local, alimentado pelas planilhas
COLETA. A publicação passa por uma etapa de anonimização com conferência
bloqueante — se sobrar qualquer identificador, o envio não acontece.
