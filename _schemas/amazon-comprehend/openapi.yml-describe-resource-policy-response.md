---
description: DescribeResourcePolicyResponse schema
layout: schema
name: DescribeResourcePolicyResponse
properties_list:
- description: ''
  name: ResourcePolicy
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: LastModifiedTime
  type: object
- description: ''
  name: PolicyRevisionId
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-describe-resource-policy-response-schema.json
slug: openapi.yml-describe-resource-policy-response
source_filename: openapi.yml-describe-resource-policy-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-resource-policy-response-schema.json\",\n  \"title\": \"DescribeResourcePolicyResponse\",\n  \"description\": \"DescribeResourcePolicyResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourcePolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Policy\"\n        },\n        {\n          \"description\": \"The JSON body of the resource-based policy.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the policy was created.\"\n        }\n      ]\n    },\n    \"LastModifiedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n\
  \        },\n        {\n          \"description\": \"The time at which the policy was last modified.\"\n        }\n      ]\n    },\n    \"PolicyRevisionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyRevisionId\"\n        },\n        {\n          \"description\": \"The revision ID of the policy. Each time you modify a policy, Amazon Comprehend assigns a new revision ID, and it deletes the prior version of the policy.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-resource-policy-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DescribeResourcePolicyResponse
---
