---
description: List of Mapping resources
layout: schema
name: MappingList
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: kind
  type: string
- description: ''
  name: metadata
  type: object
- description: List of Mapping resources
  name: items
  type: array
provider_name: Ambassador
provider_slug: ambassador
schema_file: json-schema/ambassador-mapping-list-schema.json
slug: ambassador-mapping-list
source_filename: ambassador-mapping-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MappingList\",\n  \"type\": \"object\",\n  \"description\": \"List of Mapping resources\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"type\": \"object\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"List of Mapping resources\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/json-schema/ambassador-mapping-list-schema.json
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
title: MappingList
---
