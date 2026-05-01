---
description: Settings for the action to emit HLS metadata
layout: schema
name: HlsTimedMetadataScheduleActionSettings
properties_list:
- description: ''
  name: Id3
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-hls-timed-metadata-schedule-action-settings-schema.json
slug: medialive-api-hls-timed-metadata-schedule-action-settings
source_filename: medialive-api-hls-timed-metadata-schedule-action-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-hls-timed-metadata-schedule-action-settings-schema.json\",\n  \"title\": \"HlsTimedMetadataScheduleActionSettings\",\n  \"description\": \"Settings for the action to emit HLS metadata\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id3\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id3\"\n          },\n          \"description\": \"Base64 string formatted according to the ID3 specification: http://id3.org/id3v2.4.0-structure\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Id3\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-hls-timed-metadata-schedule-action-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: HlsTimedMetadataScheduleActionSettings
---
