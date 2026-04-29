---
description: The templated target type for the EventBridge <a href="https://docs.aws.amazon.com/eventbridge/latest/APIReference/API_PutEvents.html"> <code>PutEvents</code> </a> API operation.
layout: schema
name: EventBridgeParameters
properties_list:
- description: ''
  name: DetailType
  type: object
- description: ''
  name: Source
  type: object
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-event-bridge-parameters-schema.json
slug: amazon-eventbridge-scheduler-event-bridge-parameters
source_filename: amazon-eventbridge-scheduler-event-bridge-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-event-bridge-parameters-schema.json\",\n  \"title\": \"EventBridgeParameters\",\n  \"description\": \"The templated target type for the EventBridge <a href=\\\"https://docs.aws.amazon.com/eventbridge/latest/APIReference/API_PutEvents.html\\\"> <code>PutEvents</code> </a> API operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DetailType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetailType\"\n        },\n        {\n          \"description\": \"A free-form string, with a maximum of 128 characters, used to decide what fields to expect in the event detail.\"\n        }\n      ]\n    },\n    \"Source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Source\"\n        },\n        {\n \
  \         \"description\": \"The source of the event.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DetailType\",\n    \"Source\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-event-bridge-parameters-schema.json
tags:
- Amazon Web Services
- AWS
- Cron
- Event-Driven
- Scheduling
- Serverless
title: EventBridgeParameters
---
