---
description: Allows you to configure a time window during which EventBridge Scheduler invokes the schedule.
layout: schema
name: FlexibleTimeWindow
properties_list:
- description: ''
  name: MaximumWindowInMinutes
  type: object
- description: ''
  name: Mode
  type: object
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-flexible-time-window-schema.json
slug: amazon-eventbridge-scheduler-flexible-time-window
source_filename: amazon-eventbridge-scheduler-flexible-time-window-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-flexible-time-window-schema.json\",\n  \"title\": \"FlexibleTimeWindow\",\n  \"description\": \"Allows you to configure a time window during which EventBridge Scheduler invokes the schedule.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaximumWindowInMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaximumWindowInMinutes\"\n        },\n        {\n          \"description\": \"The maximum time window during which a schedule can be invoked.\"\n        }\n      ]\n    },\n    \"Mode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FlexibleTimeWindowMode\"\n        },\n        {\n          \"description\": \"Determines whether the schedule is invoked within a flexible time window.\"\n \
  \       }\n      ]\n    }\n  },\n  \"required\": [\n    \"Mode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-flexible-time-window-schema.json
tags:
- Amazon Web Services
- Cron
- Event-Driven
- Scheduling
- Serverless
title: FlexibleTimeWindow
---
