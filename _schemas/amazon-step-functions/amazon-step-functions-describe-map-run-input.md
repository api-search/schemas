---
description: DescribeMapRunInput schema from Amazon Step Functions API
layout: schema
name: DescribeMapRunInput
properties_list:
- description: ''
  name: mapRunArn
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-describe-map-run-input-schema.json
slug: amazon-step-functions-describe-map-run-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-describe-map-run-input-schema.json\",\n  \"title\": \"DescribeMapRunInput\",\n  \"description\": \"DescribeMapRunInput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mapRunArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies a Map Run.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"mapRunArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-describe-map-run-input-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: DescribeMapRunInput
---
