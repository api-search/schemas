---
description: ClaimList schema from ACORD NGDS API
layout: schema
name: ClaimList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: pagination
  type: object
provider_name: ACORD
provider_slug: acord
schema_file: json-schema/ngds-claim-list-schema.json
slug: ngds-claim-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/ngds-claim-list-schema.json\",\n  \"title\": \"ClaimList\",\n  \"description\": \"ClaimList schema from ACORD NGDS API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Claim\"\n      }\n    },\n    \"pagination\": {\n      \"$ref\": \"#/components/schemas/Pagination\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/ngds-claim-list-schema.json
tags:
- Claims
- Insurance
- Policy
- Standards
- Underwriting
title: ClaimList
---
