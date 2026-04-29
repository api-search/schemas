---
description: ''
layout: schema
name: segment
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: footprint
  type: object
- description: ''
  name: instrumentMode
  type: string
- description: ''
  name: orderDeadline
  type: string
- description: ''
  name: extendedAngle
  type: boolean
- description: ''
  name: acquisitionStartDate
  type: string
- description: ''
  name: acquisitionEndDate
  type: string
- description: ''
  name: incidenceAngle
  type: number
- description: ''
  name: segmentKey
  type: string
- description: ''
  name: acrossTrackIncidenceAngle
  type: number
- description: ''
  name: maxIncidenceAngle
  type: number
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-segment-schema.json
slug: oneatlas-segment
source_filename: oneatlas-segment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-segment-schema.json\",\n  \"title\": \"segment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"footprint\": {\n      \"$ref\": \"#/components/schemas/footprint\"\n    },\n    \"instrumentMode\": {\n      \"type\": \"string\"\n    },\n    \"orderDeadline\": {\n      \"format\": \"datetime\",\n      \"type\": \"string\"\n    },\n    \"extendedAngle\": {\n      \"type\": \"boolean\"\n    },\n    \"acquisitionStartDate\": {\n      \"format\": \"datetime\",\n      \"type\": \"string\"\n    },\n    \"acquisitionEndDate\": {\n      \"format\": \"datetime\",\n      \"type\": \"string\"\n    },\n    \"incidenceAngle\": {\n      \"format\": \"float\",\n      \"type\": \"number\"\n    },\n    \"segmentKey\": {\n      \"type\": \"string\"\n    },\n\
  \    \"acrossTrackIncidenceAngle\": {\n      \"format\": \"float\",\n      \"type\": \"number\"\n    },\n    \"maxIncidenceAngle\": {\n      \"format\": \"float\",\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-segment-schema.json
tags:
- Imagery
- Satellites
title: segment
---
