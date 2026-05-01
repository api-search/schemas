---
description: TagResourceInput schema from Amazon EventBridge Scheduler
layout: schema
name: TagResourceInput
properties_list:
- description: ''
  name: Tags
  type: object
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-tag-resource-input-schema.json
slug: amazon-eventbridge-scheduler-tag-resource-input
source_filename: amazon-eventbridge-scheduler-tag-resource-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-tag-resource-input-schema.json\",\n  \"title\": \"TagResourceInput\",\n  \"description\": \"TagResourceInput schema from Amazon EventBridge Scheduler\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The list of tags to associate with the schedule group.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-tag-resource-input-schema.json
tags:
- Amazon Web Services
- Cron
- Event-Driven
- Scheduling
- Serverless
title: TagResourceInput
---
