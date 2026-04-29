---
description: PolicyRequest schema from ACORD NGDS API
layout: schema
name: PolicyRequest
properties_list:
- description: ''
  name: lineOfBusiness
  type: string
- description: ''
  name: effectiveDate
  type: string
- description: ''
  name: expirationDate
  type: string
- description: ''
  name: premiumAmount
  type: number
- description: ''
  name: currency
  type: string
- description: ''
  name: insuredParty
  type: object
- description: ''
  name: coverages
  type: array
provider_name: ACORD
provider_slug: acord
schema_file: json-schema/ngds-policy-request-schema.json
slug: ngds-policy-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/ngds-policy-request-schema.json\",\n  \"title\": \"PolicyRequest\",\n  \"description\": \"PolicyRequest schema from ACORD NGDS API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lineOfBusiness\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PropertyCasualty\",\n        \"Life\",\n        \"Annuity\",\n        \"Reinsurance\"\n      ]\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"expirationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"premiumAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"default\": \"USD\"\n    },\n    \"insuredParty\": {\n      \"$ref\": \"#/components/schemas/PartyRequest\"\n    },\n  \
  \  \"coverages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CoverageRequest\"\n      }\n    }\n  },\n  \"required\": [\n    \"lineOfBusiness\",\n    \"effectiveDate\",\n    \"expirationDate\",\n    \"insuredParty\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/ngds-policy-request-schema.json
tags:
- Claims
- Insurance
- Policy
- Standards
- Underwriting
title: PolicyRequest
---
