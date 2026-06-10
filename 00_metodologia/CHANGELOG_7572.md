# CHANGELOG — Refresh Ley 7572/2025 (Mercado de Valores y Productos)

Registro central da mudança de regime que afeta todo o repositório. Onde qualquer módulo citar o regime antigo do mercado de valores, vale o que está aqui.

> **Data do refresh:** jun/2026. **Verificação:** Ley 7572/2025 promulgada 07/11/2025; autoridade SIV/BCP; reglamentação em rollout faseado 2026.

---

## O que mudou (substituições globais)

| Antes (regime antigo) | Agora (Ley 7572/2025) |
|-----------------------|------------------------|
| **CNV** (Comisión Nacional de Valores) | **SIV — Superintendencia de Valores**, organismo técnico **dentro do BCP** (siv.bcp.gov.py) |
| **Ley 5810/2017** (Mercado de Valores) | **Ley 7572/2025** "Mercado de Valores y Productos" (atualiza/substitui o marco principal) |
| Leis dispersas: fundos 5452/15, bolsas de produtos 1163/97 (+5067/13), calificadoras 3899/09, securitizadoras | **Unificadas** no marco da 7572/2025 — ❓ confirmar artigo derrogatório expresso da 7572/2025 para cada uma |
| Reglamento Gral CNV CG 30/21 (+mods 31/21…35/23) | **Transitoriamente vigente** no que não contrarie a 7572/2025, até a SIV emitir a nova reglamentação |
| Autorização de Casa de Bolsa pela CNV | Autorização/registro pela **SIV** (Registro del Mercado de Valores) |
| CSD/depositária | **Caja de Valores del Paraguay S.A. (CAVAPY)** + Depositaria do BCP; sistema **Montrand** em implantação |

## Novidades materiais da 7572/2025
- **Não residente pode operar sem se constituir no país:** pessoa jurídica do exterior, registrada em mercado regulado por autoridade estrangeira reconhecida, pode fazer **emissão local de oferta pública** com requisitos de inscrição/informação. → **Alivia o gate de entrada** dos papéis investidora/emissora (Camada 2).
- **Âmbito ampliado:** valores + **produtos, serviços e atividades de investimento**; reconhece **tokenização** (tokens de direitos de crédito/propriedade/participação/investimento), **fundos privados** e **crowdfunding**.
- **Objetivo de risco sistêmico** e supervisão **baseada em risco**; alinhamento declarado a IOSCO/OCDE.
- **Regime disciplinar/penal reforçado:** tipifica oferta sem registro, manipulação de mercado, uso indevido de informação privilegiada e fraude informativo.
- **Valoração a preços de mercado** exigível aos supervisados.
- Governança: SAECA com proteção a minoritário (a reglamentar), assembleias telemáticas, ações escriturais em caja de valores, representantes de obligacionistas.

## Estado da reglamentação (jun/2026)
- ✅ Lei em vigor; SIV operando como autoridade.
- ⏳ **Reglamentos em rollout faseado 2026** ("hoja de ruta 2026"); primeira geração em emissão.
- ⚠️ **Transição:** normas antigas seguem no que não contrariem a lei nova. **Confirmar, a cada operação, qual reglamento já está vigente** (siv.bcp.gov.py / bcp.gov.py).
- ❓ Não há (ainda) reglamento general consolidado novo — não tratar como existente.

## Impacto por módulo
- **03_mercado_valores_fondos** → reescrito para o regime 7572/2025 (núcleo da mudança).
- **02_sistema_financiero_credito** → CNV→SIV nas referências; dívida pública (MEF/BCP) **não** muda.
- **04_compliance_lavado** → somar os novos tipos penais da 7572/2025.
- **06/07/08** → trocar CNV por SIV onde aparecer; resto estável.
- **11_camada2_operativa** → referências de valores/reporto/licença atualizadas; gate de não residente aliviado.
- **12_camada5_gap_reforma** → já redigida sob a 7572/2025; janela da consulta encerrada (31/12/2025) → influência migra para a 2ª geração de reglamentos.
