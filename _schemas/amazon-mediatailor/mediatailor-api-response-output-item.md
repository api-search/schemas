---
description: The output item response.
layout: schema
name: ResponseOutputItem
properties_list:
- description: ''
  name: DashPlaylistSettings
  type: object
- description: ''
  name: HlsPlaylistSettings
  type: object
- description: ''
  name: ManifestName
  type: object
- description: ''
  name: PlaybackUrl
  type: object
- description: ''
  name: SourceGroup
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-response-output-item-schema.json
slug: mediatailor-api-response-output-item
source_filename: mediatailor-api-response-output-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-response-output-item-schema.json\",\n  \"title\": \"ResponseOutputItem\",\n  \"description\": \"The output item response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DashPlaylistSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DashPlaylistSettings\"\n        },\n        {\n          \"description\": \"DASH manifest configuration settings.\"\n        }\n      ]\n    },\n    \"HlsPlaylistSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsPlaylistSettings\"\n        },\n        {\n          \"description\": \"HLS manifest configuration settings.\"\n        }\n      ]\n    },\n    \"ManifestName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n\
  \        {\n          \"description\": \"The name of the manifest for the channel that will appear in the channel output's playback URL.\"\n        }\n      ]\n    },\n    \"PlaybackUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The URL used for playback by content players.\"\n        }\n      ]\n    },\n    \"SourceGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A string used to associate a package configuration source group with a channel output.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ManifestName\",\n    \"PlaybackUrl\",\n    \"SourceGroup\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-response-output-item-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ResponseOutputItem
---
