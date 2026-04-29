---
description: DeleteResourcePolicyRequest schema from Amazon Network Firewall
layout: schema
name: DeleteResourcePolicyRequest
properties_list:
- description: ''
  name: ResourceArn
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-delete-resource-policy-request-schema.json
slug: openapi-delete-resource-policy-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-delete-resource-policy-request-schema.json\",\n  \"title\": \"DeleteResourcePolicyRequest\",\n  \"description\": \"DeleteResourcePolicyRequest schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the rule group or firewall policy whose resource policy you want to delete. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-delete-resource-policy-request-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: DeleteResourcePolicyRequest
---
