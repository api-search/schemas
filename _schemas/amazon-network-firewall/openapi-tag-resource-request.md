---
description: TagResourceRequest schema from Amazon Network Firewall
layout: schema
name: TagResourceRequest
properties_list:
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-tag-resource-request-schema.json
slug: openapi-tag-resource-request
source_filename: openapi-tag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-tag-resource-request-schema.json\",\n  \"title\": \"TagResourceRequest\",\n  \"description\": \"TagResourceRequest schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the resource.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\",\n    \"Tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-tag-resource-request-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: TagResourceRequest
---
