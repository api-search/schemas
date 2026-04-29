---
description: PutResourcePolicyInput schema
layout: schema
name: PutResourcePolicyInput
properties_list:
- description: ''
  name: policy
  type: object
- description: ''
  name: resourceArn
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-put-resource-policy-input-schema.json
slug: incident-manager-put-resource-policy-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-put-resource-policy-input-schema.json\",\n  \"title\": \"PutResourcePolicyInput\",\n  \"description\": \"PutResourcePolicyInput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Policy\"\n        },\n        {\n          \"description\": \"Details of the resource policy.\"\n        }\n      ]\n    },\n    \"resourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the response plan to add the resource policy to.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"policy\",\n    \"resourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-put-resource-policy-input-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: PutResourcePolicyInput
---
