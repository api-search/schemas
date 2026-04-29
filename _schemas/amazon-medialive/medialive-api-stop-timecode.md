---
description: Settings to identify the end of the clip.
layout: schema
name: StopTimecode
properties_list:
- description: ''
  name: LastFrameClippingBehavior
  type: object
- description: ''
  name: Timecode
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-stop-timecode-schema.json
slug: medialive-api-stop-timecode
source_filename: medialive-api-stop-timecode-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-stop-timecode-schema.json\",\n  \"title\": \"StopTimecode\",\n  \"description\": \"Settings to identify the end of the clip.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LastFrameClippingBehavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastFrameClippingBehavior\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"lastFrameClippingBehavior\"\n          },\n          \"description\": \"If you specify a StopTimecode in an input (in order to clip the file), you can specify if you want the clip to exclude (the default) or include the frame specified by the timecode.\"\n        }\n      ]\n    },\n    \"Timecode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n\
  \          \"xml\": {\n            \"name\": \"timecode\"\n          },\n          \"description\": \"The timecode for the frame where you want to stop the clip. Optional; if not specified, the clip continues to the end of the file. Enter the timecode as HH:MM:SS:FF or HH:MM:SS;FF.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-stop-timecode-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: StopTimecode
---
