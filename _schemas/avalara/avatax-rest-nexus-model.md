---
description: NexusModel schema from Avalara API
layout: schema
name: NexusModel
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: companyId
  type: integer
- description: Two-character ISO 3166 country code
  name: country
  type: string
- description: State or province code
  name: region
  type: string
- description: ''
  name: jurisTypeId
  type: string
- description: ''
  name: jurisdictionTypeId
  type: string
- description: ''
  name: jurisCode
  type: string
- description: ''
  name: jurisName
  type: string
- description: ''
  name: effectiveDate
  type: string
- description: ''
  name: endDate
  type: string
- description: ''
  name: nexusTypeId
  type: string
- description: ''
  name: hasLocalNexus
  type: boolean
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-nexus-model-schema.json
slug: avatax-rest-nexus-model
source_filename: avatax-rest-nexus-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-nexus-model-schema.json\",\n  \"title\": \"NexusModel\",\n  \"description\": \"NexusModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"companyId\": {\n      \"type\": \"integer\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Two-character ISO 3166 country code\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"State or province code\"\n    },\n    \"jurisTypeId\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"STA\",\n        \"CTY\",\n        \"CIT\",\n        \"STJ\",\n        \"CNT\"\n      ]\n    },\n    \"jurisdictionTypeId\": {\n      \"type\": \"string\"\n    },\n    \"jurisCode\": {\n      \"type\": \"string\"\n    },\n  \
  \  \"jurisName\": {\n      \"type\": \"string\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"nexusTypeId\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"None\",\n        \"SalesOrSellersUseTax\",\n        \"SalesTax\",\n        \"SSTVolunteer\",\n        \"SSTNonVolunteer\"\n      ]\n    },\n    \"hasLocalNexus\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-nexus-model-schema.json
tags:
- Taxes
title: NexusModel
---
