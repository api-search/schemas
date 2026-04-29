---
description: A StreamSelection configuration.
layout: schema
name: StreamSelection
properties_list:
- description: ''
  name: MaxVideoBitsPerSecond
  type: object
- description: ''
  name: MinVideoBitsPerSecond
  type: object
- description: ''
  name: StreamOrder
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-stream-selection-schema.json
slug: mediapackage-api-stream-selection
source_filename: mediapackage-api-stream-selection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-stream-selection-schema.json\",\n  \"title\": \"StreamSelection\",\n  \"description\": \"A StreamSelection configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxVideoBitsPerSecond\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxVideoBitsPerSecond\"\n          },\n          \"description\": \"The maximum video bitrate (bps) to include in output.\"\n        }\n      ]\n    },\n    \"MinVideoBitsPerSecond\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"minVideoBitsPerSecond\"\n          },\n          \"description\": \"The minimum video bitrate\
  \ (bps) to include in output.\"\n        }\n      ]\n    },\n    \"StreamOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamOrder\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"streamOrder\"\n          },\n          \"description\": \"A directive that determines the order of streams in the output.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-stream-selection-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: StreamSelection
---
