---
description: Settings for a SCTE-35 splice_insert message.
layout: schema
name: Scte35SpliceInsertScheduleActionSettings
properties_list:
- description: ''
  name: Duration
  type: object
- description: ''
  name: SpliceEventId
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-scte35-splice-insert-schedule-action-settings-schema.json
slug: medialive-api-scte35-splice-insert-schedule-action-settings
source_filename: medialive-api-scte35-splice-insert-schedule-action-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-splice-insert-schedule-action-settings-schema.json\",\n  \"title\": \"Scte35SpliceInsertScheduleActionSettings\",\n  \"description\": \"Settings for a SCTE-35 splice_insert message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Duration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__longMin0Max8589934591\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"duration\"\n          },\n          \"description\": \"Optional, the duration for the splice_insert, in 90 KHz ticks. To convert seconds to ticks, multiple the seconds by 90,000. If you enter a duration, there is an expectation that the downstream system can read the duration and cue in at that time. If you do not enter a duration, the splice_insert will continue indefinitely\
  \ and there is an expectation that you will enter a return_to_network to end the splice_insert at the appropriate time.\"\n        }\n      ]\n    },\n    \"SpliceEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__longMin0Max4294967295\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"spliceEventId\"\n          },\n          \"description\": \"The splice_event_id for the SCTE-35 splice_insert, as defined in SCTE-35.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SpliceEventId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-splice-insert-schedule-action-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Scte35SpliceInsertScheduleActionSettings
---
