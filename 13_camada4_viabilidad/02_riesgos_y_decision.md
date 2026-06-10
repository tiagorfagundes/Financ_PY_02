# Camada 4.2 — Riscos e Decisão (Go / No-Go)

Classificação consolidada de risco e o caminho de entrada recomendado.

---

## Classificação de risco (consolidada)

### ⚠️ BLOQUEANTES (resolver antes de operar)
1. **AML/OFAC** — qualquer contraparte/UBO sancionado inviabiliza e gera risco penal. Triagem é pré-condição, não etapa.
2. **Intermediação sem licença** — atuar como intermediária (A4) sem autorização da SIV é ilícito.
3. **"Crédito direto ao Governo"** — não existe como produto privado; usar só as portas legítimas (comprar dívida / empréstito autorizado / financiar consórcio).
4. **Repo cross-border sem netting (A3b)** — sem close-out netting oponível, o funding estrangeiro não vem ou vem caro/frágil.

### ⚠️ DEGRADAÇÃO (opera, mas com risco/custo)
5. **Dependência de reglamento 2026** (A5, C3, X2) — viabilidade real depende de texto que ainda sai; risco de cronograma.
6. **Garantia de licitação local** — exige banco local autorizado pelo BCP; custo e prazo.
7. **Liquidez secundária rasa** — preço de saída de posição é incerto (gap G2/G6).
8. **Tributação do não residente** — afeta a TIR; ainda ❓.

### 💡 MELHORIA (agenda, não impede entrar)
9. Padronização de master de repo (GMRA-like), hedge, aprofundamento do secundário.

---

## Framework de decisão (go / no-go por componente)

```
A operação como UM TODO é viável?  → NÃO como descrita ("crédito direto ao Governo").
                                       SIM se decomposta nos componentes viáveis.

Pergunta 1: A contraparte/UBO passa na triagem AML/OFAC?
   └─ NÃO → STOP (bloqueante absoluto).
   └─ SIM ↓
Pergunta 2: Qual papel nesta operação concreta?
   ├─ Investidora (conta própria)      → ✅ entra (A1/A2/A3 local, C1/C4).
   ├─ Arranjadora (sem intermediar)    → ✅ entra (C1/C2/C4), cuidar fronteira oferta pública.
   └─ Intermediária (terceiros)        → 🟡 só com licença SIV ou via parceiro licenciado.
Pergunta 3: O funding do repo vem de contraparte estrangeira?
   ├─ NÃO (local/conta própria)        → ✅ ok.
   └─ SIM                              → 🔴 trava no netting → ver P1 ou estrutura sob lei estrangeira.
Pergunta 4: Vai emitir/securitizar via oferta pública?
   └─ SIM → ⏳ depende de reglamento SIV 2026 → confirmar texto vigente.
```

---

## Caminho de entrada recomendado (faseado)

**Fase 1 — Entrar pelo núcleo viável (sem reforma):**
- Investidora em dívida soberana (A1/A2) + repo de conta própria (A3 local).
- Arranjadora de financiamento de consórcio com fideicomisso de recebíveis (C1/C4).
- Pré-requisitos: triagem AML/OFAC, custódia (CAVAPY/BCP), fechar tributação do não residente.

**Fase 2 — Escalar com licença e estrutura:**
- Obter Casa de Bolsa (SIV) **ou** parceria com casa de bolsa local → habilita A4 (intermediação) e distribuição.
- Estruturar APP/securitização conforme os reglamentos 2026 forem saindo (A5, C2, C3).

**Fase 3 — Destravar o cross-border de repo (depende de reforma):**
- A3b (funding estrangeiro contra colateral soberano) só fica robusto com **close-out netting** (P1, Camada 5).
- Aqui a empresa deixa de ser só usuária e passa a **proponente de reforma** — exatamente a finalidade do repositório.

---

## Conclusão acionável
- **Go** para Fase 1 hoje, condicionado à triagem AML e à confirmação tributária.
- **Go condicionado** para Fase 2 (licença/reglamento).
- **No-go por ora** para A3b cross-border e para "crédito direto ao Governo" — o primeiro vira go com a reforma do netting; o segundo nunca como produto privado, só reformulado.

> A viabilidade e a reforma se encontram aqui: os componentes 🔴/⏳ desta matriz **são exatamente as propostas priorizadas da Camada 5**. Operar a Fase 1 e, em paralelo, levar o pacote de reforma (netting + creadores de mercado + reglamentos SIV) é a estratégia que atende às duas finalidades do repositório — financiar agora e modernizar para financiar mais.
