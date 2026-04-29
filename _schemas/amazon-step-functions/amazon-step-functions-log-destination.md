---
description: <p/>
layout: schema
name: LogDestination
properties_list:
- description: ''
  name: cloudWatchLogsLogGroup
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-log-destination-schema.json
slug: amazon-step-functions-log-destination
source_filename: amazon-step-functions-log-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-log-destination-schema.json\",\n  \"title\": \"LogDestination\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cloudWatchLogsLogGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudWatchLogsLogGroup\"\n        },\n        {\n          \"description\": \"An object describing a CloudWatch log group. For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-logs-loggroup.html\\\">AWS::Logs::LogGroup</a> in the CloudFormation User Guide.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-log-destination-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: LogDestination
---
