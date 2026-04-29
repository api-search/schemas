---
description: ''
layout: schema
name: DimapV2PackagingParameters
properties_list:
- description: ''
  name: imageFormat
  type: string
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-dimap-v2-packaging-parameters-schema.json
slug: oneatlas-dimap-v2-packaging-parameters
source_filename: oneatlas-dimap-v2-packaging-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-dimap-v2-packaging-parameters-schema.json\",\n  \"title\": \"DimapV2PackagingParameters\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"imageFormat\": {\n      \"enum\": [\n        \"image/jp2\",\n        \"image/geotiff\"\n      ],\n      \"example\": \"image/jp2\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-dimap-v2-packaging-parameters-schema.json
tags:
- Imagery
- Satellites
title: DimapV2PackagingParameters
---
