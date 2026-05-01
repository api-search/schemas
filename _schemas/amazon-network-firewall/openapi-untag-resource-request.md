---
description: UntagResourceRequest schema from Amazon Network Firewall
layout: schema
name: UntagResourceRequest
properties_list:
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: TagKeys
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-untag-resource-request-schema.json
slug: openapi-untag-resource-request
source_filename: openapi-untag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-untag-resource-request-schema.json\",\n  \"title\": \"UntagResourceRequest\",\n  \"description\": \"UntagResourceRequest schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the resource.\"\n        }\n      ]\n    },\n    \"TagKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKeyList\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\",\n    \"TagKeys\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-untag-resource-request-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: UntagResourceRequest
---
