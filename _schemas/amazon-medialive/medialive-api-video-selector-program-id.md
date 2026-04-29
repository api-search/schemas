---
description: Video Selector Program Id
layout: schema
name: VideoSelectorProgramId
properties_list:
- description: ''
  name: ProgramId
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-video-selector-program-id-schema.json
slug: medialive-api-video-selector-program-id
source_filename: medialive-api-video-selector-program-id-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-video-selector-program-id-schema.json\",\n  \"title\": \"VideoSelectorProgramId\",\n  \"description\": \"Video Selector Program Id\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProgramId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max65536\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"programId\"\n          },\n          \"description\": \"Selects a specific program from within a multi-program transport stream. If the program doesn't exist, the first program within the transport stream will be selected by default.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-video-selector-program-id-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: VideoSelectorProgramId
---
