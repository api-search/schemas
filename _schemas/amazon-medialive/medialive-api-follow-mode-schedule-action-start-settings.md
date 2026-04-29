---
description: Settings to specify if an action follows another.
layout: schema
name: FollowModeScheduleActionStartSettings
properties_list:
- description: ''
  name: FollowPoint
  type: object
- description: ''
  name: ReferenceActionName
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-follow-mode-schedule-action-start-settings-schema.json
slug: medialive-api-follow-mode-schedule-action-start-settings
source_filename: medialive-api-follow-mode-schedule-action-start-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-follow-mode-schedule-action-start-settings-schema.json\",\n  \"title\": \"FollowModeScheduleActionStartSettings\",\n  \"description\": \"Settings to specify if an action follows another.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FollowPoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FollowPoint\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"followPoint\"\n          },\n          \"description\": \"Identifies whether this action starts relative to the start or relative to the end of the reference action.\"\n        }\n      ]\n    },\n    \"ReferenceActionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\"\
  : \"referenceActionName\"\n          },\n          \"description\": \"The action name of another action that this one refers to.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ReferenceActionName\",\n    \"FollowPoint\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-follow-mode-schedule-action-start-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: FollowModeScheduleActionStartSettings
---
