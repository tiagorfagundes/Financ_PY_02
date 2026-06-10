# Camada 4.1 — Matriz de Viabilidade

Veredito por componente da operação. Última coluna liga ao destravador (Camada 5) quando o veredito não é ✅.

---

## Eixo A — Dívida soberana

| # | Componente | Papel | Veredito | Norma que decide | Condição / ação para destravar |
|---|-----------|-------|----------|------------------|--------------------------------|
| A1 | Comprar no leilão primário | Investidora | ✅ VIÁVEL | Ley 6638/2020; 7572/2025 (não residente OK) | Custódia (CAVAPY/BCP); fechar tributação do não residente |
| A2 | Comprar/vender no secundário | Investidora | ✅ VIÁVEL (conta própria) | Reglamento 30/21 (transitório) | Operar via participante; confirmar acesso operacional do não residente |
| A3 | Repo de títulos **próprios** p/ captar funding | Investidora | 🟡 COM CONDIÇÃO | CNV 10E/15 + BVA 3090/24 (transitórios) | Conta própria com título real custodiado = OK. **Com contraparte estrangeira → trava no netting (A3b)** |
| A3b | Repo cross-border (contraparte estrangeira) | Investidora | 🔴 INVIÁVEL/FRÁGIL hoje | **Ausência de close-out netting estatutário (gap G1)** | Reforma **P1** (Camada 5) ou estruturar sob lei/jurisdição estrangeira aceita pela contraparte |
| A4 | Intermediar/distribuir p/ terceiros | Intermediária | 🟡 COM CONDIÇÃO (🔴 sem licença) | Ley 7572/2025 — autorização **SIV** | Obter **Casa de Bolsa (SIV)** OU operar via casa de bolsa local licenciada |
| A5 | Emitir valores localmente como entidade estrangeira | Emissora | ⏳ DEPENDE DE REGLAMENTO | Ley 7572/2025 (abre, mas requisitos a reglamentar) | Inscrição/informação conforme reglamento SIV 2026 — confirmar texto vigente |

## Eixo C — Consórcio / PPP

| # | Componente | Papel | Veredito | Norma que decide | Condição / ação para destravar |
|---|-----------|-------|----------|------------------|--------------------------------|
| C1 | Financiar consórcio/SPE com recebíveis do contrato | Arranjadora/Investidora | ✅ VIÁVEL | Código Civil (cessão) + Ley 921/96 (fideicomisso) | Montar fideicomisso de recebíveis; due diligence do contrato público |
| C2 | Estruturar APP com fideicomisso (AFD) | Arranjadora | 🟡 COM CONDIÇÃO | Ley 5102/13 + Dec. 1467/24 + 921/96 | Declaração de interesse público + autorização; garantia de licitação local (BCP); ⚠️ APP em possível reforma |
| C3 | Securitizar recebíveis via oferta pública | Arranjadora→Emissora | ⏳ DEPENDE DE REGLAMENTO | Ley 7572/2025 (securitizadoras/fundos) | Registro na SIV + rating; aguardar/confirmar reglamento 2026 |
| C4 | Financiamento privado/bilateral do consórcio | Investidora/credora | ✅ VIÁVEL | Código Civil + Ley 921/96 | Estruturar bilateral; **cuidar requalificação como oferta pública** |

## Transversal

| # | Componente | Veredito | Norma que decide | Reformulação |
|---|-----------|----------|------------------|--------------|
| X1 | "Emprestar crédito direto ao Governo" como produto privado | 🔴 INVIÁVEL | Ley 1535/99 + Constituição (Congresso) | Reformular: (a) comprar dívida emitida, (b) empréstito que o Estado contrate com autorização, (c) financiar o consórcio (eixo C) |
| X2 | Hedge cambial/taxa para posição em guaraníes | ⏳ DEPENDE DE REGLAMENTO | Ley 7572/2025 (negociação/compensação de derivados) | Reglamento de derivados 2026 (gap G5) |

---

## O que muda o veredito (loop com a Camada 5)

| Se for resolvido… | …destrava |
|-------------------|-----------|
| **P1 close-out netting** (reglamento derivados + lei concursal) | A3b passa de 🔴 para ✅ → repo cross-border com funding estrangeiro |
| **P2 creadores de mercado** (reglamento MEF/BCP) | A2/A3 ganham liquidez e melhor preço de saída |
| **Reglamentos SIV 2026** (intermediação, contas globais, securitização, derivados) | A4, A5, C3, X2 saem de ⏳ para ✅/🟡 |
| **P3 garantias financeiras** (execução de colateral) | A3 ganha segurança jurídica do colateral |

> Leitura estratégica: a operação **não está bloqueada** — está **escalonada**. O núcleo viável já permite entrar; o resto destrava por licença (A4), por reglamento 2026 (A5/C3/X2) ou por reforma do netting (A3b).
