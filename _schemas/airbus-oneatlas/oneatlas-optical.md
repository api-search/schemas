---
description: ''
layout: schema
name: Optical
properties_list:
- description: ''
  name: acquisitionMode
  type: string
- description: ''
  name: maxCloudCover
  type: number
- description: ''
  name: maxIncidenceAngle
  type: number
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-optical-schema.json
slug: oneatlas-optical
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-optical-schema.json\",\n  \"title\": \"Optical\",\n  \"properties\": {\n    \"acquisitionMode\": {\n      \"enum\": [\n        \"MONO\",\n        \"STEREO\",\n        \"TRISTEREO\"\n      ],\n      \"type\": \"string\"\n    },\n    \"maxCloudCover\": {\n      \"format\": \"float\",\n      \"type\": \"number\"\n    },\n    \"maxIncidenceAngle\": {\n      \"format\": \"float\",\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-optical-schema.json
tags:
- Imagery
- Satellites
title: Optical
---
