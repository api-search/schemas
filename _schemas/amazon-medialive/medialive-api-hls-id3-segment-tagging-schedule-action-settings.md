---
description: Settings for the action to insert a user-defined ID3 tag in each HLS segment
layout: schema
name: HlsId3SegmentTaggingScheduleActionSettings
properties_list:
- description: ''
  name: Tag
  type: object
- description: ''
  name: Id3
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-hls-id3-segment-tagging-schedule-action-settings-schema.json
slug: medialive-api-hls-id3-segment-tagging-schedule-action-settings
source_filename: medialive-api-hls-id3-segment-tagging-schedule-action-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-hls-id3-segment-tagging-schedule-action-settings-schema.json\",\n  \"title\": \"HlsId3SegmentTaggingScheduleActionSettings\",\n  \"description\": \"Settings for the action to insert a user-defined ID3 tag in each HLS segment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tag\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tag\"\n          },\n          \"description\": \"ID3 tag to insert into each segment. Supports special keyword identifiers to substitute in segment-related values.\\\\nSupported keyword identifiers: https://docs.aws.amazon.com/medialive/latest/ug/variable-data-identifiers.html\"\n        }\n      ]\n    },\n    \"Id3\": {\n      \"allOf\": [\n     \
  \   {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id3\"\n          },\n          \"description\": \"Base64 string formatted according to the ID3 specification: http://id3.org/id3v2.4.0-structure\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-hls-id3-segment-tagging-schedule-action-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: HlsId3SegmentTaggingScheduleActionSettings
---
