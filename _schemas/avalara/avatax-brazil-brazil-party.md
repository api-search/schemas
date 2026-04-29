---
description: BrazilParty schema from Avalara API
layout: schema
name: BrazilParty
properties_list:
- description: ''
  name: name
  type: string
- description: Company tax ID (CNPJ)
  name: cnpj
  type: string
- description: Individual tax ID (CPF)
  name: cpf
  type: string
- description: Inscricao Estadual
  name: stateRegistration
  type: string
- description: Inscricao Municipal
  name: municipalRegistration
  type: string
- description: ''
  name: address
  type: object
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-brazil-brazil-party-schema.json
slug: avatax-brazil-brazil-party
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-brazil-brazil-party-schema.json\",\n  \"title\": \"BrazilParty\",\n  \"description\": \"BrazilParty schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"cnpj\": {\n      \"type\": \"string\",\n      \"description\": \"Company tax ID (CNPJ)\"\n    },\n    \"cpf\": {\n      \"type\": \"string\",\n      \"description\": \"Individual tax ID (CPF)\"\n    },\n    \"stateRegistration\": {\n      \"type\": \"string\",\n      \"description\": \"Inscricao Estadual\"\n    },\n    \"municipalRegistration\": {\n      \"type\": \"string\",\n      \"description\": \"Inscricao Municipal\"\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"street\": {\n          \"type\": \"string\"\n        },\n   \
  \     \"number\": {\n          \"type\": \"string\"\n        },\n        \"complement\": {\n          \"type\": \"string\"\n        },\n        \"neighborhood\": {\n          \"type\": \"string\"\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"cityCode\": {\n          \"type\": \"string\",\n          \"description\": \"IBGE city code\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"State code (UF)\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\"\n        },\n        \"country\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-brazil-brazil-party-schema.json
tags:
- Taxes
title: BrazilParty
---
