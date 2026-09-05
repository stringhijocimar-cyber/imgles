# ProcureAI — Supplier Cost & Negotiation Intelligence

ProcureAI é um SaaS enxuto para compradores, gestores de procurement e pequenas/médias empresas analisarem propostas de fornecedores, reajustes de preço, composição de custos e oportunidades de saving.

## Problema

Equipes de compras frequentemente trabalham com Excel, e-mail e análises manuais para:
- comparar fornecedores;
- avaliar reajustes;
- calcular impacto anual;
- analisar markup e composição de custos;
- construir contrapropostas;
- documentar savings e cost avoidance.

## Proposta de valor

O usuário importa uma planilha ou cadastra itens manualmente. O sistema calcula automaticamente:
- preço atual x proposto;
- variação absoluta e percentual;
- impacto anual;
- composição de custo;
- markup estimado;
- preço-alvo por margem configurável;
- saving potencial;
- ranking de fornecedores;
- recomendação de negociação.

## Público-alvo

- compradores e analistas de procurement;
- consultores de sourcing;
- pequenas e médias indústrias;
- empresas automotivas, metalúrgicas, mineração e manutenção industrial;
- gestores que ainda dependem fortemente de Excel.

## Monetização sugerida

### Free
- até 20 itens por análise;
- 3 análises/mês;
- dashboard básico.

### Pro — R$ 49,90/mês
- análises ilimitadas;
- exportação Excel/PDF;
- histórico;
- cenários de negociação;
- dashboards avançados.

### Business — R$ 149,90/mês
- até 5 usuários;
- banco de fornecedores;
- projetos de sourcing;
- aprovação interna;
- indicadores de saving.

### Consultor — R$ 249,90/mês
- múltiplos clientes;
- relatórios white-label;
- exportação executiva;
- gestão de projetos de negociação.

## MVP

1. Dashboard.
2. Cadastro/importação de itens.
3. Comparação preço atual x novo.
4. Breakdown de custo.
5. Markup e preço-alvo.
6. Saving potencial.
7. Simulador de contraproposta.
8. Exportação de relatório.

## Diferencial competitivo

Não tentar substituir SAP, Coupa ou grandes suites de procurement. O foco é ser a camada de inteligência de negociação que hoje vive em planilhas.

## Stack sugerida

- Frontend: Next.js + TypeScript + Tailwind
- Backend: Supabase/PostgreSQL
- Auth: Supabase Auth
- Pagamentos: Stripe ou Mercado Pago
- Charts: Recharts
- Importação: XLSX
- Deploy: Vercel

## Próximos passos

- construir MVP funcional;
- validar com 5 compradores;
- liberar plano gratuito;
- medir conversão para Pro;
- incluir IA para recomendações de negociação após validação do fluxo básico.
