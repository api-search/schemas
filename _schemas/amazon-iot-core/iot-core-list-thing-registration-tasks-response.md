---
description: ListThingRegistrationTasksResponse schema
layout: schema
name: ListThingRegistrationTasksResponse
properties_list:
- description: ''
  name: taskIds
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-list-thing-registration-tasks-response-schema.json
slug: iot-core-list-thing-registration-tasks-response
source_filename: iot-core-list-thing-registration-tasks-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-thing-registration-tasks-response-schema.json\",\n  \"title\": \"ListThingRegistrationTasksResponse\",\n  \"description\": \"ListThingRegistrationTasksResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskIdList\"\n        },\n        {\n          \"description\": \"A list of bulk thing provisioning task IDs.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to use to get the next set of results, or <b>null</b> if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-thing-registration-tasks-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: ListThingRegistrationTasksResponse
---
