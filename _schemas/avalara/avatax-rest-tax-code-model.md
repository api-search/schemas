---
description: TaxCodeModel schema from Avalara API
layout: schema
name: TaxCodeModel
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: companyId
  type: integer
- description: ''
  name: taxCode
  type: string
- description: ''
  name: taxCodeTypeId
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: isPhysical
  type: boolean
- description: ''
  name: isActive
  type: boolean
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-tax-code-model-schema.json
slug: avatax-rest-tax-code-model
source_filename: avatax-rest-tax-code-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-tax-code-model-schema.json\",\n  \"title\": \"TaxCodeModel\",\n  \"description\": \"TaxCodeModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"companyId\": {\n      \"type\": \"integer\"\n    },\n    \"taxCode\": {\n      \"type\": \"string\"\n    },\n    \"taxCodeTypeId\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"isPhysical\": {\n      \"type\": \"boolean\"\n    },\n    \"isActive\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-tax-code-model-schema.json
tags:
- Taxes
title: TaxCodeModel
---
