---
description: DescribeActivityInput schema from Amazon Step Functions API
layout: schema
name: DescribeActivityInput
properties_list:
- description: ''
  name: activityArn
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-describe-activity-input-schema.json
slug: amazon-step-functions-describe-activity-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-describe-activity-input-schema.json\",\n  \"title\": \"DescribeActivityInput\",\n  \"description\": \"DescribeActivityInput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"activityArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the activity to describe.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"activityArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-describe-activity-input-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: DescribeActivityInput
---
