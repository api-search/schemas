---
description: GetResourcePoliciesOutput schema
layout: schema
name: GetResourcePoliciesOutput
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: resourcePolicies
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-get-resource-policies-output-schema.json
slug: incident-manager-get-resource-policies-output
source_filename: incident-manager-get-resource-policies-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-get-resource-policies-output-schema.json\",\n  \"title\": \"GetResourcePoliciesOutput\",\n  \"description\": \"GetResourcePoliciesOutput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The pagination token to continue to the next page of results.\"\n        }\n      ]\n    },\n    \"resourcePolicies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourcePolicyList\"\n        },\n        {\n          \"description\": \"Details about the resource policy attached to the response plan.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourcePolicies\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-get-resource-policies-output-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: GetResourcePoliciesOutput
---
