---
description: The configuration for HLS content.
layout: schema
name: HlsConfiguration
properties_list:
- description: ''
  name: ManifestEndpointPrefix
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-hls-configuration-schema.json
slug: mediatailor-api-hls-configuration
source_filename: mediatailor-api-hls-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-hls-configuration-schema.json\",\n  \"title\": \"HlsConfiguration\",\n  \"description\": \"The configuration for HLS content.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ManifestEndpointPrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The URL that is used to initiate a playback session for devices that support Apple HLS. The session uses server-side reporting.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-hls-configuration-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: HlsConfiguration
---
