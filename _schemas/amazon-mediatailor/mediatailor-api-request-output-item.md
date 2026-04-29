---
description: The output configuration for this channel.
layout: schema
name: RequestOutputItem
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
  name: SourceGroup
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-request-output-item-schema.json
slug: mediatailor-api-request-output-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-request-output-item-schema.json\",\n  \"title\": \"RequestOutputItem\",\n  \"description\": \"The output configuration for this channel.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DashPlaylistSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DashPlaylistSettings\"\n        },\n        {\n          \"description\": \"DASH manifest configuration parameters.\"\n        }\n      ]\n    },\n    \"HlsPlaylistSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsPlaylistSettings\"\n        },\n        {\n          \"description\": \"HLS playlist configuration parameters.\"\n        }\n      ]\n    },\n    \"ManifestName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"description\": \"The name of the manifest for the channel. The name appears in the <code>PlaybackUrl</code>.\"\n        }\n      ]\n    },\n    \"SourceGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A string used to match which <code>HttpPackageConfiguration</code> is used for each <code>VodSource</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ManifestName\",\n    \"SourceGroup\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-request-output-item-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: RequestOutputItem
---
