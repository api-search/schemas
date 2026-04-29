---
description: PolicyList schema from ACORD NGDS API
layout: schema
name: PolicyList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: pagination
  type: object
provider_name: ACORD
provider_slug: acord
schema_file: json-schema/ngds-policy-list-schema.json
slug: ngds-policy-list
source_filename: ngds-policy-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/ngds-policy-list-schema.json\",\n  \"title\": \"PolicyList\",\n  \"description\": \"PolicyList schema from ACORD NGDS API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Policy\"\n      }\n    },\n    \"pagination\": {\n      \"$ref\": \"#/components/schemas/Pagination\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/ngds-policy-list-schema.json
tags:
- Claims
- Insurance
- Policy
- Standards
- Underwriting
title: PolicyList
---
