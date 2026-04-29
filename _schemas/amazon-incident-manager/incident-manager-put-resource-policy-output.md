---
description: PutResourcePolicyOutput schema
layout: schema
name: PutResourcePolicyOutput
properties_list:
- description: ''
  name: policyId
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-put-resource-policy-output-schema.json
slug: incident-manager-put-resource-policy-output
source_filename: incident-manager-put-resource-policy-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-put-resource-policy-output-schema.json\",\n  \"title\": \"PutResourcePolicyOutput\",\n  \"description\": \"PutResourcePolicyOutput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyId\"\n        },\n        {\n          \"description\": \"The ID of the resource policy.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"policyId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-put-resource-policy-output-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: PutResourcePolicyOutput
---
