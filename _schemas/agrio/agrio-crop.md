---
description: A supported agricultural crop type.
layout: schema
name: Crop
properties_list:
- description: Unique crop identifier.
  name: id
  type: string
- description: Common name for the crop.
  name: common_name
  type: string
- description: Scientific name for the crop.
  name: scientific_name
  type: string
provider_name: agrio
provider_slug: agrio
schema_file: json-schema/agrio-crop-schema.json
slug: agrio-crop
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/json-schema/agrio-crop-schema.json\",\n  \"title\": \"Crop\",\n  \"description\": \"A supported agricultural crop type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique crop identifier.\",\n      \"example\": \"tomato\"\n    },\n    \"common_name\": {\n      \"type\": \"string\",\n      \"description\": \"Common name for the crop.\",\n      \"example\": \"Tomato\"\n    },\n    \"scientific_name\": {\n      \"type\": \"string\",\n      \"description\": \"Scientific name for the crop.\",\n      \"example\": \"Solanum lycopersicum\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/json-schema/agrio-crop-schema.json
tags:
- Agriculture
- Plant Disease
- Pest Detection
- AI
- Crop Advisory
title: Crop
---
