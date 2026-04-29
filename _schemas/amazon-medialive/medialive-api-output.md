---
description: Output settings. There can be multiple outputs within a group.
layout: schema
name: Output
properties_list:
- description: ''
  name: AudioDescriptionNames
  type: object
- description: ''
  name: CaptionDescriptionNames
  type: object
- description: ''
  name: OutputName
  type: object
- description: ''
  name: OutputSettings
  type: object
- description: ''
  name: VideoDescriptionName
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-output-schema.json
slug: medialive-api-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-output-schema.json\",\n  \"title\": \"Output\",\n  \"description\": \"Output settings. There can be multiple outputs within a group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioDescriptionNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioDescriptionNames\"\n          },\n          \"description\": \"The names of the AudioDescriptions used as audio sources for this output.\"\n        }\n      ]\n    },\n    \"CaptionDescriptionNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"captionDescriptionNames\"\n          },\n    \
  \      \"description\": \"The names of the CaptionDescriptions used as caption sources for this output.\"\n        }\n      ]\n    },\n    \"OutputName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max255\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputName\"\n          },\n          \"description\": \"The name used to identify an output.\"\n        }\n      ]\n    },\n    \"OutputSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputSettings\"\n          },\n          \"description\": \"Output type-specific settings.\"\n        }\n      ]\n    },\n    \"VideoDescriptionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"videoDescriptionName\"\n          },\n          \"description\"\
  : \"The name of the VideoDescription used as the source for this output.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"OutputSettings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-output-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Output
---
