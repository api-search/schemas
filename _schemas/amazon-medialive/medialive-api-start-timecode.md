---
description: Settings to identify the start of the clip.
layout: schema
name: StartTimecode
properties_list:
- description: ''
  name: Timecode
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-start-timecode-schema.json
slug: medialive-api-start-timecode
source_filename: medialive-api-start-timecode-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-start-timecode-schema.json\",\n  \"title\": \"StartTimecode\",\n  \"description\": \"Settings to identify the start of the clip.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Timecode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timecode\"\n          },\n          \"description\": \"The timecode for the frame where you want to start the clip. Optional; if not specified, the clip starts at first frame in the file. Enter the timecode as HH:MM:SS:FF or HH:MM:SS;FF.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-start-timecode-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: StartTimecode
---
