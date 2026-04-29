---
description: Filters evaluation results based on start and end times.
layout: schema
name: TimeWindow
properties_list:
- description: ''
  name: StartTime
  type: object
- description: ''
  name: EndTime
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-time-window-schema.json
slug: config-time-window
source_filename: config-time-window-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-time-window-schema.json\",\n  \"title\": \"TimeWindow\",\n  \"description\": \"Filters evaluation results based on start and end times.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The start time of an execution.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The end time of an execution. The end time must be after the start date.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-time-window-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: TimeWindow
---
