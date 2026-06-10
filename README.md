# Arcabouço Legal — Operações Financeiras no Paraguai

Repositório de base normativa e metodologia jurisprudencial para **estudos de viabilidade operacional** de operações financeiras (públicas e privadas, internas e transfronteiriças) no Paraguai.

> **Escopo coberto:** contratos financeiros públicos e privados · operações de crédito interno e externo · compliance de entidades financeiras e fundos · licitações/contratações públicas · APP, consórcios e grupos econômicos · mercado de valores e fundos de investimento.

---

## ⚠️ Advertências de uso (leia antes)

> **🔄 Refresh Ley 7572/2025:** o regime do mercado de valores mudou (CNV→SIV, 5810/17→7572/2025). Mudanças globais documentadas em [00_metodologia/CHANGELOG_7572.md](00_metodologia/CHANGELOG_7572.md).


1. **Isto NÃO é um repositório "completo" nem aconselhamento jurídico.** É um mapa de fontes primárias verificadas + metodologia. Direito paraguaio muda; a fonte oficial sempre prevalece sobre este resumo. Para uma operação real, valide cada norma na BACN/BCP/DNCP e com advogado habilitado no Paraguai.
2. **Vigência:** cada norma listada tem data e principais modificadoras *conhecidas até a verificação*. Antes de fechar uma operação, cheque modificações posteriores no Digesto Legislativo e na BACN.
3. **"Ministerio de Hacienda" → MEF.** A reforma de 2023-2024 transformou o Ministério da Fazenda em **Ministerio de Economía y Finanzas (MEF)**. Textos legais antigos ainda dizem "Hacienda"; leia como MEF onde for órgão reitor.
4. **Mercado de valores — NOVO MARCO (Ley 7572/2025).** A transição se consolidou: a **Ley 7572/2025 "Mercado de Valores y Productos"** (promulgada 07/11/2025) unificou o regime e tornou o **BCP, via Superintendencia de Valores (SIV)**, a autoridade única, derrogando/absorvendo leis anteriores (incl. partes da 5810/17). Os módulos 03 e a Camada 2 referenciam o regime antigo e **precisam de refresh** para a 7572/2025 — ver `12_camada5_gap_reforma/`.
5. **Jurisprudência:** este repo **não cita Acuerdos y Sentencias específicos** porque não foram verificados em fonte primária. O módulo `09_jurisprudencia/` traz **onde e como buscar**, não casos fabricados.

---

## Hierarquia normativa paraguaia (ordem de prelação)

```
Constitución Nacional (1992)
   └─ Tratados internacionais ratificados (art. 137, 141 CN)
        └─ Leyes del Congreso
             └─ Decretos do Poder Executivo (reglamentarios)
                  └─ Resoluciones de órgãos reguladores (BCP, CNV, SEPRELAD, DNCP, CONACOM)
                       └─ Circulares / atos administrativos
```
Para o sistema financeiro especificamente, a Ley 861/96 fixa prelação própria: Ley 861/96 → Ley Orgánica del BCP (489/95) → Código Civil (1183/85) → demais leis.

---

## Mapa rápido: domínio → norma central → regulador

| # | Domínio | Norma(s) central(is) verificada(s) | Regulador / autoridade |
|---|---------|-----------------------------------|------------------------|
| 01 | Base civil e contratual | **Ley 1183/85 (Código Civil)**; Ley 1034/83 "Del Comerciante" | Poder Judicial |
| 02 | Banco Central e política monetária/cambial | **Ley 489/95** Orgánica BCP, mod./ampl. por **Ley 6104/2018** | BCP |
| 02 | Bancos, financeiras, crédito | **Ley 861/96**, mod. por **Ley 5787/16** (e outras) | BCP / Superintendencia de Bancos |
| 02 | Banca de fomento (2º piso) | **Ley 2640/2005** (AFD), mod./ampl. por **Ley 6769/2021** (abroga 3330/2007) | AFD |
| 02 | Garantia de depósitos / resolução bancária | Lei de Garantía de Depósitos (FGD) — *verificar nº atual* | BCP |
| 02 | Dados creditícios / informação privada | **Ley 1682/01**, mod. por **Ley 1969/02** (e atualizações) | — |
| 03 | Mercado de valores e produtos | **Ley 7572/2025** (substitui 5810/17; unifica o setor) | **SIV** (Superintendencia de Valores, no BCP) |
| 03 | Fundos de investimento | Absorvido pela **Ley 7572/2025** (ex-5452/15); + fundos privados/crowdfunding | SIV |
| 03 | Bolsas de produtos | Absorvido pela **Ley 7572/2025** (ex-1163/97 + 5067/13) | SIV |
| 03 | Agências de rating / securitizadoras | Absorvido pela **Ley 7572/2025** (ex-3899/09) | SIV |
| 04 | Lavagem / financiamento do terrorismo | **Ley 1015/97**, mod. por **3783/09, 6497/19, 6797/21, 6960/22** | SEPRELAD (UIF) |
| 04 | Imobilização de ativos (terrorismo/ADM) | **Ley 6419/2019** | SEPRELAD |
| 04 | Terrorismo e financiamento (penal) | **Ley 4024/2010** | MP / Judiciário |
| 05 | Contratações públicas / licitações | **Ley 7021/2022** (deroga 2051/03); Dec. **9823/2023** + Dec. **2264/2024** | DNCP + MEF |
| 06 | Aliança público-privada (APP) | **Ley 5102/2013**, regul. por Dec. **1467/2024** (substitui 4183/2020 e 1350/14) | Unidade APP / MEF / DNCP |
| 06 | Fideicomisso / negócios fiduciários | **Ley 921/96** "De Negocios Fiduciarios" | BCP / SIV conforme tipo |
| 06 | Obras "llave en mano" / financiamento alternativo | **Ley 5074/2013** | MEF / MOPC |
| 08 | Defesa da concorrência / grupos econômicos | **Ley 4956/2013**, regul. por Dec. **1490/2014** | CONACOM |

> Detalhe de cada linha, com artigos-chave, limiares e links oficiais, nos arquivos das pastas correspondentes.

---

## Estrutura do repositório

```
repo-legal-py/
├── README.md                         ← este arquivo (índice-mestre)
├── 00_metodologia/                   ← fontes oficiais, como verificar vigência
├── 01_constitucional_civil/          ← base contratual e societária
├── 02_sistema_financiero_credito/    ← BCP, bancos, AFD, crédito púb./priv., dívida
├── 03_mercado_valores_fondos/        ← valores, fundos, bolsas, rating
├── 04_compliance_lavado/             ← AML/CFT, sujeitos obrigados, OFAC/sanções
├── 05_contrataciones_publicas/       ← Ley 7021/2022 e regulamentos
├── 06_app_proyectos_fideicomiso/     ← APP, fideicomisso, llave en mano
├── 07_consorcios_grupos_sociedades/  ← consórcios, sociedades, grupos
├── 08_defensa_competencia/           ← controle de concentrações, condutas
├── 09_jurisprudencia/                ← METODOLOGIA + repositórios oficiais
└── 10_viabilidad_operacional/        ← checklist operacional acionável
```

### Navegação rápida
- 🚀 **Comece aqui:** [Checklist de Viabilidade Operacional](10_viabilidad_operacional/checklist.md)
- [00 · Metodologia e Fontes Oficiais](00_metodologia/fuentes.md)
- [01 · Base Constitucional e Civil](01_constitucional_civil/base.md)
- [02 · Sistema Financeiro e Crédito](02_sistema_financiero_credito/marco.md)
- [03 · Mercado de Valores e Fundos](03_mercado_valores_fondos/marco.md)
- [04 · Compliance AML/CFT](04_compliance_lavado/marco.md)
- [05 · Contratações Públicas](05_contrataciones_publicas/marco.md)
- [06 · APP, Fideicomisso e Projetos](06_app_proyectos_fideicomiso/marco.md)
- [07 · Consórcios, Sociedades e Grupos](07_consorcios_grupos_sociedades/marco.md)
- [08 · Defesa da Concorrência](08_defensa_competencia/marco.md)
- [09 · Jurisprudência (metodologia)](09_jurisprudencia/metodologia.md)

### Camada 2 — Operativa (operação de dívida pública)
- 🧱 [Camada 2 · Regulatória Operativa](11_camada2_operativa/00_README_camada2.md) — emissão, repo/colateral, licenças (3 papéis), consórcio/PPP, cross-border/AML

### Camada 5 — Gap Analysis e Reforma
- 🎯 [Camada 5 · Gap Analysis e Propostas de Reforma](12_camada5_gap_reforma/00_README_camada5.md) — gaps vs. mercados maduros, propostas priorizadas e a janela regulatória da Ley 7572/2025

### Camada 4 — Matriz de Viabilidade
- ✅ [Camada 4 · Matriz de Viabilidade](13_camada4_viabilidad/00_README_camada4.md) — veredito (viável / com condição / depende de reglamento / inviável) por eixo, papel e estrutura, com go/no-go *(pasta nº 13; construída após a Camada 5)*

---

## Estado de verificação

| Status | Significado |
|--------|-------------|
| ✅ VERIFICADO | número, título e data conferidos em fonte oficial/secundária confiável nesta sessão |
| ⚠️ VERIFICAR VIGÊNCIA | norma existe mas há sinal de reforma/transição recente — confirmar antes de usar |
| ❓ PENDENTE | mencionado mas não confirmado número/artigo exato — não usar sem checar |

Última verificação de fontes: ver [00_metodologia/fuentes.md](00_metodologia/fuentes.md).

---

## Manutenção
- Ao revisar uma norma, atualize o status (✅/⚠️/❓) e a data no módulo correspondente.
- Reformas em acompanhamento: **APP (Ley 5102/13)** e **autoridade do mercado de valores (CNV ↔ Superintendencia de Valores/BCP)**.
- Para virar instrumento de uma operação concreta, aprofunde o módulo aplicável e puxe jurisprudência real por [09_jurisprudencia](09_jurisprudencia/metodologia.md).

## Licença
Sem licença definida. Defina uma antes de tornar o repo público (ex.: `CC-BY-4.0` para conteúdo documental, ou `MIT` se preferir permissivo). Sem licença explícita, "todos os direitos reservados" se aplica por padrão.
