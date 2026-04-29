---
description: Coverage schema from ACORD NGDS API
layout: schema
name: Coverage
properties_list:
- description: ''
  name: coverageId
  type: string
- description: ''
  name: coverageType
  type: string
- description: ''
  name: limit
  type: number
- description: ''
  name: deductible
  type: number
- description: ''
  name: premium
  type: number
- description: ''
  name: currency
  type: string
provider_name: ACORD
provider_slug: acord
schema_file: json-schema/ngds-coverage-schema.json
slug: ngds-coverage
source_filename: ngds-coverage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/ngds-coverage-schema.json\",\n  \"title\": \"Coverage\",\n  \"description\": \"Coverage schema from ACORD NGDS API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"coverageId\": {\n      \"type\": \"string\"\n    },\n    \"coverageType\": {\n      \"type\": \"string\"\n    },\n    \"limit\": {\n      \"type\": \"number\"\n    },\n    \"deductible\": {\n      \"type\": \"number\"\n    },\n    \"premium\": {\n      \"type\": \"number\"\n    },\n    \"currency\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/ngds-coverage-schema.json
tags:
- Claims
- Insurance
- Policy
- Standards
- Underwriting
title: Coverage
---
