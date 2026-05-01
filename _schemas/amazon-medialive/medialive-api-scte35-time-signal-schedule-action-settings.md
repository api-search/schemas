---
description: Settings for a SCTE-35 time_signal.
layout: schema
name: Scte35TimeSignalScheduleActionSettings
properties_list:
- description: ''
  name: Scte35Descriptors
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-scte35-time-signal-schedule-action-settings-schema.json
slug: medialive-api-scte35-time-signal-schedule-action-settings
source_filename: medialive-api-scte35-time-signal-schedule-action-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-time-signal-schedule-action-settings-schema.json\",\n  \"title\": \"Scte35TimeSignalScheduleActionSettings\",\n  \"description\": \"Settings for a SCTE-35 time_signal.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Scte35Descriptors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfScte35Descriptor\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte35Descriptors\"\n          },\n          \"description\": \"The list of SCTE-35 descriptors accompanying the SCTE-35 time_signal.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Scte35Descriptors\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-time-signal-schedule-action-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Scte35TimeSignalScheduleActionSettings
---
