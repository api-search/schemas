---
description: Settings to specify when an action should occur. Only one of the options must be selected.
layout: schema
name: ScheduleActionStartSettings
properties_list:
- description: ''
  name: FixedModeScheduleActionStartSettings
  type: object
- description: ''
  name: FollowModeScheduleActionStartSettings
  type: object
- description: ''
  name: ImmediateModeScheduleActionStartSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-schedule-action-start-settings-schema.json
slug: medialive-api-schedule-action-start-settings
source_filename: medialive-api-schedule-action-start-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-schedule-action-start-settings-schema.json\",\n  \"title\": \"ScheduleActionStartSettings\",\n  \"description\": \"Settings to specify when an action should occur. Only one of the options must be selected.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FixedModeScheduleActionStartSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FixedModeScheduleActionStartSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fixedModeScheduleActionStartSettings\"\n          },\n          \"description\": \"Option for specifying the start time for an action.\"\n        }\n      ]\n    },\n    \"FollowModeScheduleActionStartSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FollowModeScheduleActionStartSettings\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"followModeScheduleActionStartSettings\"\n          },\n          \"description\": \"Option for specifying an action as relative to another action.\"\n        }\n      ]\n    },\n    \"ImmediateModeScheduleActionStartSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImmediateModeScheduleActionStartSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"immediateModeScheduleActionStartSettings\"\n          },\n          \"description\": \"Option for specifying an action that should be applied immediately.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-schedule-action-start-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ScheduleActionStartSettings
---
