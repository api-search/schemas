---
description: <p/>
layout: schema
name: CloudWatchLogsLogGroup
properties_list:
- description: ''
  name: logGroupArn
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-cloud-watch-logs-log-group-schema.json
slug: amazon-step-functions-cloud-watch-logs-log-group
source_filename: amazon-step-functions-cloud-watch-logs-log-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-cloud-watch-logs-log-group-schema.json\",\n  \"title\": \"CloudWatchLogsLogGroup\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"logGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the the CloudWatch log group to which you want your logs emitted to. The ARN must end with <code>:*</code> \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-cloud-watch-logs-log-group-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: CloudWatchLogsLogGroup
---
