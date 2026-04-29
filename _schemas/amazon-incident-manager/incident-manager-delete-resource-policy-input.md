---
description: DeleteResourcePolicyInput schema
layout: schema
name: DeleteResourcePolicyInput
properties_list:
- description: ''
  name: policyId
  type: object
- description: ''
  name: resourceArn
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-delete-resource-policy-input-schema.json
slug: incident-manager-delete-resource-policy-input
source_filename: incident-manager-delete-resource-policy-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-delete-resource-policy-input-schema.json\",\n  \"title\": \"DeleteResourcePolicyInput\",\n  \"description\": \"DeleteResourcePolicyInput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyId\"\n        },\n        {\n          \"description\": \"The ID of the resource policy you're deleting.\"\n        }\n      ]\n    },\n    \"resourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the resource you're deleting the policy from.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"policyId\",\n    \"resourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-delete-resource-policy-input-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: DeleteResourcePolicyInput
---
