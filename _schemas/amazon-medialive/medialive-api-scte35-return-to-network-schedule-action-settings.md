---
description: Settings for a SCTE-35 return_to_network message.
layout: schema
name: Scte35ReturnToNetworkScheduleActionSettings
properties_list:
- description: ''
  name: SpliceEventId
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-scte35-return-to-network-schedule-action-settings-schema.json
slug: medialive-api-scte35-return-to-network-schedule-action-settings
source_filename: medialive-api-scte35-return-to-network-schedule-action-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-return-to-network-schedule-action-settings-schema.json\",\n  \"title\": \"Scte35ReturnToNetworkScheduleActionSettings\",\n  \"description\": \"Settings for a SCTE-35 return_to_network message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SpliceEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__longMin0Max4294967295\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"spliceEventId\"\n          },\n          \"description\": \"The splice_event_id for the SCTE-35 splice_insert, as defined in SCTE-35.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SpliceEventId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-return-to-network-schedule-action-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Scte35ReturnToNetworkScheduleActionSettings
---
