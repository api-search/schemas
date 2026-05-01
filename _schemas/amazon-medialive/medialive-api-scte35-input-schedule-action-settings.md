---
description: Scte35Input Schedule Action Settings
layout: schema
name: Scte35InputScheduleActionSettings
properties_list:
- description: ''
  name: InputAttachmentNameReference
  type: object
- description: ''
  name: Mode
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-scte35-input-schedule-action-settings-schema.json
slug: medialive-api-scte35-input-schedule-action-settings
source_filename: medialive-api-scte35-input-schedule-action-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-input-schedule-action-settings-schema.json\",\n  \"title\": \"Scte35InputScheduleActionSettings\",\n  \"description\": \"Scte35Input Schedule Action Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputAttachmentNameReference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputAttachmentNameReference\"\n          },\n          \"description\": \"In fixed mode, enter the name of the input attachment that you want to use as a SCTE-35 input. (Don't enter the ID of the input.)\\\"\"\n        }\n      ]\n    },\n    \"Mode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scte35InputMode\"\n        },\n        {\n          \"xml\"\
  : {\n            \"name\": \"mode\"\n          },\n          \"description\": \"Whether the SCTE-35 input should be the active input or a fixed input.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Mode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-input-schedule-action-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Scte35InputScheduleActionSettings
---
