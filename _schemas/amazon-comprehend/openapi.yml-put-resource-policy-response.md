---
description: PutResourcePolicyResponse schema
layout: schema
name: PutResourcePolicyResponse
properties_list:
- description: ''
  name: PolicyRevisionId
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-put-resource-policy-response-schema.json
slug: openapi.yml-put-resource-policy-response
source_filename: openapi.yml-put-resource-policy-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-put-resource-policy-response-schema.json\",\n  \"title\": \"PutResourcePolicyResponse\",\n  \"description\": \"PutResourcePolicyResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PolicyRevisionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyRevisionId\"\n        },\n        {\n          \"description\": \"The revision ID of the policy. Each time you modify a policy, Amazon Comprehend assigns a new revision ID, and it deletes the prior version of the policy.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-put-resource-policy-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: PutResourcePolicyResponse
---
