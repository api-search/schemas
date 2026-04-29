---
description: ''
layout: schema
name: pixelCoding
properties_list:
- description: ''
  name: key
  type: object
- description: Defines the pixel coding. <br>'8bits' when radiometric_processing = 'display'<br>, '12bits' otherwise
  name: value
  type: object
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-pixel-coding-schema.json
slug: oneatlas-pixel-coding
source_filename: oneatlas-pixel-coding-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-pixel-coding-schema.json\",\n  \"title\": \"pixelCoding\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"enum\": [\n        \"pixel_coding\"\n      ]\n    },\n    \"value\": {\n      \"enum\": [\n        \"8bits\",\n        \"12bits\"\n      ],\n      \"description\": \"Defines the pixel coding. <br>'8bits' when radiometric_processing = 'display'<br>, '12bits' otherwise\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-pixel-coding-schema.json
tags:
- Imagery
- Satellites
title: pixelCoding
---
