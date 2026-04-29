---
description: 'Settings for the "switch input" action: to switch from ingesting one input to ingesting another input.'
layout: schema
name: InputSwitchScheduleActionSettings
properties_list:
- description: ''
  name: InputAttachmentNameReference
  type: object
- description: ''
  name: InputClippingSettings
  type: object
- description: ''
  name: UrlPath
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-switch-schedule-action-settings-schema.json
slug: medialive-api-input-switch-schedule-action-settings
source_filename: medialive-api-input-switch-schedule-action-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-switch-schedule-action-settings-schema.json\",\n  \"title\": \"InputSwitchScheduleActionSettings\",\n  \"description\": \"Settings for the \\\"switch input\\\" action: to switch from ingesting one input to ingesting another input.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputAttachmentNameReference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputAttachmentNameReference\"\n          },\n          \"description\": \"The name of the input attachment (not the name of the input!) to switch to. The name is specified in the channel configuration.\"\n        }\n      ]\n    },\n    \"InputClippingSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/InputClippingSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputClippingSettings\"\n          },\n          \"description\": \"Settings to let you create a clip of the file input, in order to set up the input to ingest only a portion of the file.\"\n        }\n      ]\n    },\n    \"UrlPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"urlPath\"\n          },\n          \"description\": \"The value for the variable portion of the URL for the dynamic input, for this instance of the input. Each time you use the same dynamic input in an input switch action, you can provide a different value, in order to connect the input to a different content source.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InputAttachmentNameReference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-switch-schedule-action-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: InputSwitchScheduleActionSettings
---
