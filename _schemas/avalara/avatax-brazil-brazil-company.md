---
description: BrazilCompany schema from Avalara API
layout: schema
name: BrazilCompany
properties_list:
- description: ''
  name: companyId
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: cnpj
  type: string
- description: ''
  name: stateRegistration
  type: string
- description: ''
  name: municipalRegistration
  type: string
- description: ''
  name: taxRegime
  type: string
- description: ''
  name: state
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-brazil-brazil-company-schema.json
slug: avatax-brazil-brazil-company
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-brazil-brazil-company-schema.json\",\n  \"title\": \"BrazilCompany\",\n  \"description\": \"BrazilCompany schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"companyId\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"cnpj\": {\n      \"type\": \"string\"\n    },\n    \"stateRegistration\": {\n      \"type\": \"string\"\n    },\n    \"municipalRegistration\": {\n      \"type\": \"string\"\n    },\n    \"taxRegime\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SimplesNacional\",\n        \"LucroPresumido\",\n        \"LucroReal\"\n      ]\n    },\n    \"state\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-brazil-brazil-company-schema.json
tags:
- Taxes
title: BrazilCompany
---
