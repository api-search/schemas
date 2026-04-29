---
description: Placeholder documentation for InputSpecification
layout: schema
name: InputSpecification
properties_list:
- description: ''
  name: Codec
  type: object
- description: ''
  name: MaximumBitrate
  type: object
- description: ''
  name: Resolution
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-specification-schema.json
slug: medialive-api-input-specification
source_filename: medialive-api-input-specification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-specification-schema.json\",\n  \"title\": \"InputSpecification\",\n  \"description\": \"Placeholder documentation for InputSpecification\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Codec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputCodec\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codec\"\n          },\n          \"description\": \"Input codec\"\n        }\n      ]\n    },\n    \"MaximumBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputMaximumBitrate\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maximumBitrate\"\n          },\n          \"description\": \"Maximum input bitrate, categorized coarsely\"\n        }\n      ]\n    },\n    \"\
  Resolution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputResolution\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"resolution\"\n          },\n          \"description\": \"Input resolution, categorized coarsely\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-specification-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: InputSpecification
---
