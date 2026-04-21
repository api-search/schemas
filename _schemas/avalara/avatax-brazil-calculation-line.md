---
description: CalculationLine schema from Avalara API
layout: schema
name: CalculationLine
properties_list:
- description: ''
  name: lineCode
  type: string
- description: ''
  name: itemCode
  type: string
- description: ''
  name: numberOfItems
  type: number
- description: ''
  name: lineAmount
  type: number
- description: ''
  name: itemDescription
  type: string
- description: NCM (Nomenclatura Comum do Mercosul) code
  name: ncmCode
  type: string
- description: CST (Codigo de Situacao Tributaria) code
  name: cstCode
  type: string
- description: CFOP (Codigo Fiscal de Operacoes e Prestacoes) code
  name: cfopCode
  type: string
- description: Origin state code (UF)
  name: originState
  type: string
- description: Destination state code (UF)
  name: destinationState
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-brazil-calculation-line-schema.json
slug: avatax-brazil-calculation-line
tags:
- Taxes
title: CalculationLine
---
