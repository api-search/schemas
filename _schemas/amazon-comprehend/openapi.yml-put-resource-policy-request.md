---
description: PutResourcePolicyRequest schema
layout: schema
name: PutResourcePolicyRequest
properties_list:
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: ResourcePolicy
  type: object
- description: ''
  name: PolicyRevisionId
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-put-resource-policy-request-schema.json
slug: openapi.yml-put-resource-policy-request
source_filename: openapi.yml-put-resource-policy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-put-resource-policy-request-schema.json\",\n  \"title\": \"PutResourcePolicyRequest\",\n  \"description\": \"PutResourcePolicyRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendModelArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the custom model to attach the policy to.\"\n        }\n      ]\n    },\n    \"ResourcePolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Policy\"\n        },\n        {\n          \"description\": \"<p>The JSON resource-based policy to attach to your custom model. Provide your JSON as a UTF-8 encoded string without line breaks. To provide valid JSON for your policy,\
  \ enclose the attribute names and values in double quotes. If the JSON body is also enclosed in double quotes, then you must escape the double quotes that are inside the policy:</p> <p> <code>\\\"{\\\\\\\"attribute\\\\\\\": \\\\\\\"value\\\\\\\", \\\\\\\"attribute\\\\\\\": [\\\\\\\"value\\\\\\\"]}\\\"</code> </p> <p>To avoid escaping quotes, you can use single quotes to enclose the policy and double quotes to enclose the JSON names and values:</p> <p> <code>'{\\\"attribute\\\": \\\"value\\\", \\\"attribute\\\": [\\\"value\\\"]}'</code> </p>\"\n        }\n      ]\n    },\n    \"PolicyRevisionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyRevisionId\"\n        },\n        {\n          \"description\": \"The revision ID that Amazon Comprehend assigned to the policy that you are updating. If you are creating a new policy that has no prior version, don't use this parameter. Amazon Comprehend creates the revision ID for you.\"\n        }\n      ]\n \
  \   }\n  },\n  \"required\": [\n    \"ResourceArn\",\n    \"ResourcePolicy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-put-resource-policy-request-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: PutResourcePolicyRequest
---
