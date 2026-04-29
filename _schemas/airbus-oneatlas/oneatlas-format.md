---
description: ''
layout: schema
name: Format
properties_list:
- description: ''
  name: checksum
  type: object
- description: ''
  name: compression
  type: string
- description: ''
  name: packaging
  type: object
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-format-schema.json
slug: oneatlas-format
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-format-schema.json\",\n  \"title\": \"Format\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checksum\": {\n      \"properties\": {\n        \"parameters\": {\n          \"example\": {\n            \"crcCode\": \"dhdf54\"\n          },\n          \"oneOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Md5ChecksumParameters\"\n            }\n          ]\n        },\n        \"type\": {\n          \"enum\": [\n            \"md5\",\n            \"none\"\n          ],\n          \"type\": \"string\"\n        }\n      },\n      \"type\": \"object\"\n    },\n    \"compression\": {\n      \"enum\": [\n        \"zip\"\n      ],\n      \"type\": \"string\"\n    },\n    \"packaging\": {\n      \"properties\": {\n        \"parameters\": {\n          \"description\": \"Key/value\
  \ options of the packaging. Properties depend on the type of packaging\",\n          \"example\": {\n            \"imageFormat\": \"image/jp2\"\n          },\n          \"oneOf\": [\n            {\n              \"$ref\": \"#/components/schemas/DimapV2PackagingParameters\"\n            }\n          ]\n        },\n        \"type\": {\n          \"enum\": [\n            \"dimapV2\"\n          ],\n          \"type\": \"string\"\n        }\n      },\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-format-schema.json
tags:
- Imagery
- Satellites
title: Format
---
