---
description: Settings to let you create a clip of the file input, in order to set up the input to ingest only a portion of the file.
layout: schema
name: InputClippingSettings
properties_list:
- description: ''
  name: InputTimecodeSource
  type: object
- description: ''
  name: StartTimecode
  type: object
- description: ''
  name: StopTimecode
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-clipping-settings-schema.json
slug: medialive-api-input-clipping-settings
source_filename: medialive-api-input-clipping-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-clipping-settings-schema.json\",\n  \"title\": \"InputClippingSettings\",\n  \"description\": \"Settings to let you create a clip of the file input, in order to set up the input to ingest only a portion of the file.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputTimecodeSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputTimecodeSource\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputTimecodeSource\"\n          },\n          \"description\": \"The source of the timecodes in the source being clipped.\"\n        }\n      ]\n    },\n    \"StartTimecode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StartTimecode\"\n        },\n        {\n          \"xml\": {\n           \
  \ \"name\": \"startTimecode\"\n          },\n          \"description\": \"Settings to identify the start of the clip.\"\n        }\n      ]\n    },\n    \"StopTimecode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StopTimecode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"stopTimecode\"\n          },\n          \"description\": \"Settings to identify the end of the clip.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InputTimecodeSource\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-clipping-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: InputClippingSettings
---
