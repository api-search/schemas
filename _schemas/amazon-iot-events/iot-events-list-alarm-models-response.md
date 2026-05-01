---
description: ListAlarmModelsResponse schema
layout: schema
name: ListAlarmModelsResponse
properties_list:
- description: ''
  name: alarmModelSummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-list-alarm-models-response-schema.json
slug: iot-events-list-alarm-models-response
source_filename: iot-events-list-alarm-models-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-list-alarm-models-response-schema.json\",\n  \"title\": \"ListAlarmModelsResponse\",\n  \"description\": \"ListAlarmModelsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alarmModelSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmModelSummaries\"\n        },\n        {\n          \"description\": \"A list that summarizes each alarm model.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token that you can use to return the next set of results, or <code>null</code> if there are no more results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-list-alarm-models-response-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: ListAlarmModelsResponse
---
