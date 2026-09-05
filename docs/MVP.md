# ProcureAI — Escopo do MVP

## Fluxo principal

1. Criar conta.
2. Criar projeto de negociação.
3. Importar Excel/CSV ou incluir itens manualmente.
4. Informar preço atual, preço proposto, volume anual e custos conhecidos.
5. Visualizar impacto financeiro e oportunidade.
6. Definir margem/markup-alvo.
7. Gerar contraproposta item a item.
8. Exportar relatório executivo.

## Entidades principais

### Project
- id
- name
- supplier_name
- category
- buyer
- currency
- created_at

### Item
- part_number
- description
- annual_volume
- current_price
- proposed_price
- material_cost
- process_cost
- third_party_cost
- logistics_cost
- other_cost

### Calculated fields
- current_annual_spend
- proposed_annual_spend
- delta_unit
- delta_percent
- total_known_cost
- estimated_markup_percent
- target_price
- potential_saving_unit
- potential_saving_annual

## Fórmulas iniciais

current_annual_spend = current_price * annual_volume

proposed_annual_spend = proposed_price * annual_volume

delta_unit = proposed_price - current_price

delta_percent = (proposed_price / current_price - 1) * 100

total_known_cost = material_cost + process_cost + third_party_cost + logistics_cost + other_cost

estimated_markup_percent = ((proposed_price / total_known_cost) - 1) * 100

target_price = total_known_cost * (1 + target_markup_percent / 100)

potential_saving_unit = proposed_price - target_price

potential_saving_annual = potential_saving_unit * annual_volume

## Dashboard

KPIs:
- Spend atual anual
- Spend proposto anual
- Impacto do reajuste
- Saving potencial
- % médio solicitado
- % médio recomendado

Gráficos:
- Top 10 itens por impacto anual
- Breakdown de custos
- Solicitação vs contraproposta
- Saving por fornecedor/projeto

## Regras comerciais do MVP

- O sistema não substitui ERP.
- Não executar pagamentos.
- Não emitir pedido de compra.
- Não armazenar dados bancários.
- Priorizar análise e decisão.

## Critério de sucesso do MVP

O usuário deve conseguir transformar uma planilha de reajuste em uma recomendação objetiva de negociação em menos de 10 minutos.
