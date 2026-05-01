---
description: CreateProtectionRequest schema from api
layout: schema
name: CreateProtectionRequest
properties_list:
- description: ''
  name: Name
  type: string
- description: ''
  name: ResourceArn
  type: string
- description: ''
  name: Tags
  type: array
provider_name: Amazon Shield
provider_slug: amazon-shield
schema_file: json-schema/amazon-shield-api-create-protection-request-schema.json
slug: amazon-shield-api-create-protection-request
source_filename: amazon-shield-api-create-protection-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/json-schema/amazon-shield-api-create-protection-request-schema.json\",\n  \"title\": \"CreateProtectionRequest\",\n  \"description\": \"CreateProtectionRequest schema from api\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\"\n    },\n    \"ResourceArn\": {\n      \"type\": \"string\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tag\"\n      }\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"ResourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/json-schema/amazon-shield-api-create-protection-request-schema.json
tags:
- DDoS Protection
- Networking
- Security
title: CreateProtectionRequest
---
