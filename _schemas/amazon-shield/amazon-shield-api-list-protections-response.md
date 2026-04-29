---
description: ListProtectionsResponse schema from api
layout: schema
name: ListProtectionsResponse
properties_list:
- description: ''
  name: Protections
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon Shield
provider_slug: amazon-shield
schema_file: json-schema/amazon-shield-api-list-protections-response-schema.json
slug: amazon-shield-api-list-protections-response
source_filename: amazon-shield-api-list-protections-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/json-schema/amazon-shield-api-list-protections-response-schema.json\",\n  \"title\": \"ListProtectionsResponse\",\n  \"description\": \"ListProtectionsResponse schema from api\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Protections\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Protection\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/json-schema/amazon-shield-api-list-protections-response-schema.json
tags:
- AWS
- DDoS Protection
- Networking
- Security
title: ListProtectionsResponse
---
