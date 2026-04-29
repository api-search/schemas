---
description: TaxRuleModel schema from Avalara API
layout: schema
name: TaxRuleModel
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: companyId
  type: integer
- description: ''
  name: taxCodeId
  type: integer
- description: ''
  name: taxCode
  type: string
- description: ''
  name: stateFIPS
  type: string
- description: ''
  name: jurisName
  type: string
- description: ''
  name: jurisCode
  type: string
- description: ''
  name: jurisTypeId
  type: string
- description: ''
  name: rateTypeId
  type: string
- description: ''
  name: ruleTypeId
  type: string
- description: ''
  name: isAllJuris
  type: boolean
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-tax-rule-model-schema.json
slug: avatax-rest-tax-rule-model
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-tax-rule-model-schema.json\",\n  \"title\": \"TaxRuleModel\",\n  \"description\": \"TaxRuleModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"companyId\": {\n      \"type\": \"integer\"\n    },\n    \"taxCodeId\": {\n      \"type\": \"integer\"\n    },\n    \"taxCode\": {\n      \"type\": \"string\"\n    },\n    \"stateFIPS\": {\n      \"type\": \"string\"\n    },\n    \"jurisName\": {\n      \"type\": \"string\"\n    },\n    \"jurisCode\": {\n      \"type\": \"string\"\n    },\n    \"jurisTypeId\": {\n      \"type\": \"string\"\n    },\n    \"rateTypeId\": {\n      \"type\": \"string\"\n    },\n    \"ruleTypeId\": {\n      \"type\": \"string\"\n    },\n    \"isAllJuris\": {\n      \"type\": \"boolean\"\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-tax-rule-model-schema.json
tags:
- Taxes
title: TaxRuleModel
---
