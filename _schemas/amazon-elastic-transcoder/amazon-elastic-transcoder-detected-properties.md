---
description: The detected properties of the input file. Elastic Transcoder identifies these values from the input file.
layout: schema
name: DetectedProperties
properties_list:
- description: ''
  name: Width
  type: object
- description: ''
  name: Height
  type: object
- description: ''
  name: FrameRate
  type: object
- description: ''
  name: FileSize
  type: object
- description: ''
  name: DurationMillis
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-detected-properties-schema.json
slug: amazon-elastic-transcoder-detected-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-detected-properties-schema.json\",\n  \"title\": \"DetectedProperties\",\n  \"description\": \"The detected properties of the input file. Elastic Transcoder identifies these values from the input file.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Width\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"The detected width of the input file, in pixels.\"\n        }\n      ]\n    },\n    \"Height\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"The detected height of the input file, in pixels.\"\n        }\n      ]\n    },\n    \"FrameRate\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/FloatString\"\n        },\n        {\n          \"description\": \"The detected frame rate of the input file, in frames per second.\"\n        }\n      ]\n    },\n    \"FileSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableLong\"\n        },\n        {\n          \"description\": \"The detected file size of the input file, in bytes.\"\n        }\n      ]\n    },\n    \"DurationMillis\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableLong\"\n        },\n        {\n          \"description\": \"The detected duration of the input file, in milliseconds.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-detected-properties-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: DetectedProperties
---
