# Camada 2.2 — Mercado Secundário, Reporto e Colateral

> 🔄 **Refresh 7572/2025:** autoridade do mercado de valores = **SIV** (ex-CNV), no BCP. Ver `00_metodologia/CHANGELOG_7572.md`.

O coração da "monetização legítima": usar títulos de dívida pública reais e custodiados como ativo para captar funding (repo/colateralização) e repassar crédito.

---

## Negociabilidade do título (pré-condição)
- A **Depositaria de Valores do BCP** está interconectada com a **BVA**, permitindo a negociabilidade de Bonos del Tesoro no mercado de valores. Sem custódia/anotação em conta, não há repo nem colateral eficaz.
- Títulos desmaterializados → transferência por anotação em conta.

## Reporto (repo) — o trilho normativo
- **CNV Res. N° 10 E/15 (20/01/2015)** — aprova o **reglamento de negociação de Operações de Reporto** via sistema eletrônico de negociação.
- **BVA Res. 3090/24** — define o reporto: o **reportado vende** valores ao **reportador** por prazo determinado a preço inicial; o reportador adquire os valores (anotação em conta) **até o vencimento**, quando se desfaz a operação (recompra). Estrutura clássica de **sell-buyback**.
- **Reglamento General del Mercado de Valores (CNV CG 30/21 e mods)** — trata as posições de reporto no cálculo de **Cartera Propia** da casa de bolsa (efeito prudencial/capital): distingue reporto ≤ 3 dias e > 3 dias, e quem atua como reportador (prestamista) vs. reportado (prestatario).

> Tradução para a operação: a empresa que detém um Bono del Tesoro pode **levantar funding** entregando-o em reporto (vende com recompra), e usar esse caixa para **repassar crédito** — tudo com título real, custodiado e precificado. É a forma legítima do que você chamou de "monetizar".

## Colateral e liquidação (Sistema Nacional de Pagos)
- **Ley 7503/2025 — Sistema Nacional de Pagos** — define, para os sistemas administrados pelo BCP, que servem de **garantia** os títulos emitidos pelo BCP, pelo **Tesouro Público**, e os de entidades públicas com garantia do Tesouro, além de dinheiro e títulos conforme regulamentação.
- Liquidação bruta em tempo real (LBTR/RTGS) e ordens de transferência de fundos e valores.

> Consequência: o **Bono del Tesoro é colateral elegível** no sistema de pagamentos/garantias do BCP — base para repo, garantias intradía e colateralização robusta.

## Operação extrabursátil (OTC)
- O Reglamento (art. 8) admite **operação extrabursátil** — fora da bolsa local, no mercado local ou no exterior — desde que com **intermediário de valores autorizado pela SIV**, por conta de terceiros ou por conta própria. Relevante para estruturas OTC e cross-border do repo.

---

## Pontos de atenção
- ⚠️ **BLOQUEANTE de papel:** para fazer reporto/intermediação desses títulos por conta de terceiros, é preciso ser (ou operar via) **intermediário autorizado pela SIV** — ver arquivo 03. Por conta própria com recursos próprios há mais espaço, mas confirmar enquadramento.
- ⚠️ **Risco de reprecificação/haircut:** repo expõe a marcação a mercado e haircut; modelar margem e chamada de margem no contrato.
- ⚠️ **Padronização contratual:** PY não tem (confirmar) um master agreement de repo no padrão **GMRA/ICMA**; isso vira ponto de gap analysis (Camada 5) e risco de execução de garantia.
- ❓ Confirmar se o repo sobre títulos públicos tem tratamento específico além do reglamento (CNV 30/21 transitório → SIV) (eventual circular do BCP).
