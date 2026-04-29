---
description: The parameters for using an CloudWatch Logs log stream as a target.
layout: schema
name: PipeTargetCloudWatchLogsParameters
properties_list:
- description: ''
  name: LogStreamName
  type: object
- description: ''
  name: Timestamp
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-pipe-target-cloud-watch-logs-parameters-schema.json
slug: amazon-eventbridge-pipes-pipe-target-cloud-watch-logs-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-cloud-watch-logs-parameters-schema.json\",\n  \"title\": \"PipeTargetCloudWatchLogsParameters\",\n  \"description\": \"The parameters for using an CloudWatch Logs log stream as a target.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LogStreamName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogStreamName\"\n        },\n        {\n          \"description\": \"The name of the log stream.\"\n        }\n      ]\n    },\n    \"Timestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JsonPath\"\n        },\n        {\n          \"description\": \"The time the event occurred, expressed as the number of milliseconds after Jan 1, 1970 00:00:00 UTC.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-cloud-watch-logs-parameters-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: PipeTargetCloudWatchLogsParameters
---
