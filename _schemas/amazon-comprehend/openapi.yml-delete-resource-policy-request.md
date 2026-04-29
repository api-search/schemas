---
description: DeleteResourcePolicyRequest schema
layout: schema
name: DeleteResourcePolicyRequest
properties_list:
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: PolicyRevisionId
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-delete-resource-policy-request-schema.json
slug: openapi.yml-delete-resource-policy-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-delete-resource-policy-request-schema.json\",\n  \"title\": \"DeleteResourcePolicyRequest\",\n  \"description\": \"DeleteResourcePolicyRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendModelArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the custom model version that has the policy to delete.\"\n        }\n      ]\n    },\n    \"PolicyRevisionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyRevisionId\"\n        },\n        {\n          \"description\": \"The revision ID of the policy to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-delete-resource-policy-request-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DeleteResourcePolicyRequest
---
