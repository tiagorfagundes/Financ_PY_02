# 00 — Metodologia e Fontes Oficiais

## Como este repositório foi montado

1. Toda norma foi confirmada contra **fonte primária (texto da lei)** ou fonte secundária confiável (firmas jurídicas, reguladores).
2. Números, títulos e modificadoras são marcados ✅ / ⚠️ / ❓ conforme o nível de confirmação.
3. **Nada de jurisprudência sem fonte.** Casos concretos só entram se puxados dos repositórios oficiais (ver `09_jurisprudencia/`).

## Portais oficiais para verificar VIGÊNCIA (sempre prevalecem sobre este repo)

| Fonte | O que tem | Domínio |
|-------|-----------|---------|
| **BACN** — bacn.gov.py/leyes-paraguayas | Texto oficial das leis (Biblioteca y Archivo del Congreso) | Tudo |
| **Digesto Legislativo** — digestolegislativo.gov.py | Estado de vigência, derrogações, modificações | Tudo |
| **SILpy** — silpy.congreso.gov.py | Tramitação e projetos de lei em curso | Reformas pendentes |
| **Gaceta Oficial** — gacetaoficial.gov.py | Publicação oficial (vigência começa aqui) | Tudo |
| **BCP** — bcp.gov.py/leyes | Leis e resoluções do sistema financeiro | 02, 03, 04 |
| **SIV** (Superintendencia de Valores) — siv.bcp.gov.py | Resoluções do mercado de valores e fundos (ex-CNV) | 03 |
| **SEPRELAD** — seprelad.gov.py | Resoluções AML/CFT por tipo de sujeito obrigado | 04 |
| **DNCP** — contrataciones.gov.py | Ley 7021, decretos, pliegos, registro de fornecedores | 05, 06 |
| **CONACOM** (sob MIC) — mic.gov.py/conacom | Defesa da concorrência, concentrações | 08 |
| **Poder Judicial** — pj.gov.py | Jurisprudência, Gaceta Judicial | 09 |

## Princípio operacional para o estudo de viabilidade

> **Confirmar antes de citar.** Para uma operação real, cada norma usada no parecer deve ser reaberta na BACN/Digesto na data do parecer. Reforma silenciosa (decreto regulamentar novo) é a causa mais comum de erro — vide o caso da Ley 2051/03, substituída integralmente pela Ley 7021/22 em vigor plena desde 19/02/2024.

## Separação fato confirmado × afirmação não verificada (regra do repo)

- **FATO CONFIRMADO:** número + título + data conferidos.
- **INFERÊNCIA:** consequência lógica de norma confirmada, mas não literal — marcar como tal.
- **NÃO VERIFICADO:** sinalizar ❓ e não usar como base de decisão.
