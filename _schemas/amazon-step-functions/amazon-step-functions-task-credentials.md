---
description: Contains details about the credentials that Step Functions uses for a task.
layout: schema
name: TaskCredentials
properties_list:
- description: ''
  name: roleArn
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-task-credentials-schema.json
slug: amazon-step-functions-task-credentials
source_filename: amazon-step-functions-task-credentials-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-task-credentials-schema.json\",\n  \"title\": \"TaskCredentials\",\n  \"description\": \"Contains details about the credentials that Step Functions uses for a task.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongArn\"\n        },\n        {\n          \"description\": \"The ARN of an IAM role that Step Functions assumes for the task. The role can allow cross-account access to resources.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-task-credentials-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: TaskCredentials
---
