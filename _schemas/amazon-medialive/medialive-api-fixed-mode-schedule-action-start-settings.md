---
description: Start time for the action.
layout: schema
name: FixedModeScheduleActionStartSettings
properties_list:
- description: ''
  name: Time
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-fixed-mode-schedule-action-start-settings-schema.json
slug: medialive-api-fixed-mode-schedule-action-start-settings
source_filename: medialive-api-fixed-mode-schedule-action-start-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-fixed-mode-schedule-action-start-settings-schema.json\",\n  \"title\": \"FixedModeScheduleActionStartSettings\",\n  \"description\": \"Start time for the action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Time\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"time\"\n          },\n          \"description\": \"Start time for the action to start in the channel. (Not the time for the action to be added to the schedule: actions are always added to the schedule immediately.) UTC format: yyyy-mm-ddThh:mm:ss.nnnZ. All the letters are digits (for example, mm might be 01) except for the two constants \\\"T\\\" for time and \\\"Z\\\" for \\\"UTC format\\\".\"\n        }\n   \
  \   ]\n    }\n  },\n  \"required\": [\n    \"Time\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-fixed-mode-schedule-action-start-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: FixedModeScheduleActionStartSettings
---
