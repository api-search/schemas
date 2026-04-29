---
description: ListJobExecutionsForThingResponse schema
layout: schema
name: ListJobExecutionsForThingResponse
properties_list:
- description: ''
  name: executionSummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-list-job-executions-for-thing-response-schema.json
slug: iot-core-list-job-executions-for-thing-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-job-executions-for-thing-response-schema.json\",\n  \"title\": \"ListJobExecutionsForThingResponse\",\n  \"description\": \"ListJobExecutionsForThingResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"executionSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobExecutionSummaryForThingList\"\n        },\n        {\n          \"description\": \"A list of job execution summaries.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token for the next set of results, or <b>null</b> if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-job-executions-for-thing-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: ListJobExecutionsForThingResponse
---
