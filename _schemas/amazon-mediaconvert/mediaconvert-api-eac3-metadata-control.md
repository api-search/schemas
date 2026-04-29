---
description: When set to FOLLOW_INPUT, encoder metadata will be sourced from the DD, DD+, or DolbyE decoder that supplied this audio data. If audio was not supplied from one of these streams, then the static metadata settings will be used.
layout: schema
name: Eac3MetadataControl
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-eac3-metadata-control-schema.json
slug: mediaconvert-api-eac3-metadata-control
source_filename: mediaconvert-api-eac3-metadata-control-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-eac3-metadata-control-schema.json\",\n  \"title\": \"Eac3MetadataControl\",\n  \"description\": \"When set to FOLLOW_INPUT, encoder metadata will be sourced from the DD, DD+, or DolbyE decoder that supplied this audio data. If audio was not supplied from one of these streams, then the static metadata settings will be used.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"FOLLOW_INPUT\",\n    \"USE_CONFIGURED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-eac3-metadata-control-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Eac3MetadataControl
---
