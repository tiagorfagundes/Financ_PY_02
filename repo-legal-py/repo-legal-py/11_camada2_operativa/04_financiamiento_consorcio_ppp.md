# Camada 2.4 — Financiamento de Consórcio / PPP (eixo C)

> 🔄 **Refresh 7572/2025:** autoridade do mercado de valores = **SIV** (ex-CNV), no BCP. Ver `00_metodologia/CHANGELOG_7572.md`.

Eixo C operativo: financiar o consórcio que detém (ou disputa) contrato público/PPP, com os recebíveis do contrato e/ou títulos como ativo. Aqui o tomador é o consórcio/SPE, **não** o Estado diretamente.

---

## Estrutura jurídica do veículo
- **APP (Ley 5102/2013, regul. Decreto 1467/2024):** contrato de longo prazo; o adjudicatário constitui **Sociedade de Objeto Específico (SPE)** (art. 27) e usa **fideicomisso**.
- **Fideicomisso (Ley 921/96):** patrimônio autônomo, separado dos sócios — base do ring-fencing. Na APP, o **Fundo de Garantia e Liquidez** é administrado pela **AFD** como fiduciária.
- **Consórcio (Ley 7021/22 / 5102/13):** admite consórcio; atenção à **responsabilidade solidária** dos consorciados perante o Estado (módulo 07).

## Fontes de repagamento (o "ativo" que se financia)
1. **Recebíveis do contrato público/PPP** — os pagamentos do Estado ao contrato. Cessão/cessão fiduciária de recebíveis (Código Civil + 921/96) para o fideicomisso, que serve a dívida.
2. **Títulos soberanos** dados em garantia/repo (arquivo 02) para liquidez da SPE.
3. **Combinação:** fideicomisso recebe recebíveis + colateral em títulos → emite dívida/cotas → capta com investidores (eixo A).

## Como securitizar / captar
- Se a captação for **oferta pública** (bonos da SPE, cotas de fundo) → entra no **mercado de valores** (Ley 7572/2025; Reglamento CNV 30/21 transitório) e exige estrutura registrada na **SIV** + (provável) **rating** (regime de calificadoras absorvido pela 7572/2025).
- Se for **privada/bilateral** → contrato direto + fideicomisso, fora da oferta pública (cuidar para não requalificar como oferta pública).
- **Fundos (Ley 5452/15):** veículo possível para empacotar e distribuir.

## Garantias na licitação (gate prático para estrangeiro)
- Garantia de manutenção de oferta (Dec. 9823/23): **banco local autorizado pelo BCP** ou seguradora local de caução. **Banco estrangeiro não serve direto** — planejar emissão local (módulo 05 do repo).

---

## Fluxo-tipo (eixo C + A combinados)
```
Estado (contratante)  ──pagamentos do contrato──►  Fideicomisso (AFD ou privado)
       ▲                                                   │
       │ executa obra/serviço                              │ serve a dívida / distribui
   Consórcio/SPE  ◄── crédito/funding ──  Investidores (eixo A) ◄── repo de títulos (arquivo 02)
```

## Pontos de atenção
- ⚠️ **BLOQUEANTE:** garantia de licitação tem de vir de banco local autorizado pelo BCP — custo/prazo no cronograma.
- ⚠️ **Solidariedade do consórcio:** uma parte responde pelas demais perante o Estado.
- ⚠️ **Oferta pública disfarçada:** captação "privada" que atinge o público é requalificável pela SIV — risco de nulidade/sanção.
- ⚠️ **APP em reforma:** projeto de modernização da Ley 5102/13 em tramitação — verificar antes de estruturar (módulo 06).
- 💡 O fideicomisso (921/96) é o ponto de articulação entre eixo C (recebíveis) e eixo A (títulos/repo). É onde a operação ganha robustez de ring-fencing.
