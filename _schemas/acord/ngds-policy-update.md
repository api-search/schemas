---
description: PolicyUpdate schema from ACORD NGDS API
layout: schema
name: PolicyUpdate
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: expirationDate
  type: string
- description: ''
  name: premiumAmount
  type: number
- description: ''
  name: endorsements
  type: array
provider_name: ACORD
provider_slug: acord
schema_file: json-schema/ngds-policy-update-schema.json
slug: ngds-policy-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/ngds-policy-update-schema.json\",\n  \"title\": \"PolicyUpdate\",\n  \"description\": \"PolicyUpdate schema from ACORD NGDS API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Active\",\n        \"Lapsed\",\n        \"Cancelled\",\n        \"Pending\",\n        \"Expired\"\n      ]\n    },\n    \"expirationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"premiumAmount\": {\n      \"type\": \"number\"\n    },\n    \"endorsements\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"endorsementNumber\": {\n            \"type\": \"string\"\n          },\n          \"description\": {\n            \"type\": \"string\"\n          },\n    \
  \      \"effectiveDate\": {\n            \"type\": \"string\",\n            \"format\": \"date\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/ngds-policy-update-schema.json
tags:
- Claims
- Insurance
- Policy
- Standards
- Underwriting
title: PolicyUpdate
---
