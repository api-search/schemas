---
description: ExciseLicense schema from Avalara API
layout: schema
name: ExciseLicense
properties_list:
- description: ''
  name: licenseId
  type: string
- description: ''
  name: licenseNumber
  type: string
- description: ''
  name: licenseType
  type: string
- description: ''
  name: issuingJurisdiction
  type: string
- description: ''
  name: effectiveDate
  type: string
- description: ''
  name: expirationDate
  type: string
- description: ''
  name: status
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/excise-excise-license-schema.json
slug: excise-excise-license
source_filename: excise-excise-license-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-excise-license-schema.json\",\n  \"title\": \"ExciseLicense\",\n  \"description\": \"ExciseLicense schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"licenseId\": {\n      \"type\": \"string\"\n    },\n    \"licenseNumber\": {\n      \"type\": \"string\"\n    },\n    \"licenseType\": {\n      \"type\": \"string\"\n    },\n    \"issuingJurisdiction\": {\n      \"type\": \"string\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"expirationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Active\",\n        \"Expired\",\n        \"Suspended\",\n        \"Revoked\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-excise-license-schema.json
tags:
- Taxes
title: ExciseLicense
---
