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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-brazil-calculation-line-schema.json\",\n  \"title\": \"CalculationLine\",\n  \"description\": \"CalculationLine schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lineCode\": {\n      \"type\": \"string\"\n    },\n    \"itemCode\": {\n      \"type\": \"string\"\n    },\n    \"numberOfItems\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"lineAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"itemDescription\": {\n      \"type\": \"string\"\n    },\n    \"ncmCode\": {\n      \"type\": \"string\",\n      \"description\": \"NCM (Nomenclatura Comum do Mercosul) code\"\n    },\n    \"cstCode\": {\n      \"type\": \"string\",\n      \"description\": \"CST (Codigo de Situacao Tributaria) code\"\n    },\n    \"cfopCode\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"CFOP (Codigo Fiscal de Operacoes e Prestacoes) code\"\n    },\n    \"originState\": {\n      \"type\": \"string\",\n      \"description\": \"Origin state code (UF)\"\n    },\n    \"destinationState\": {\n      \"type\": \"string\",\n      \"description\": \"Destination state code (UF)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-brazil-calculation-line-schema.json
tags:
- Taxes
title: CalculationLine
---
