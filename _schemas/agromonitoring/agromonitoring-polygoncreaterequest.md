---
description: Request body for creating a new field polygon.
layout: schema
name: PolygonCreateRequest
properties_list:
- description: Display name for the field.
  name: name
  type: string
- description: ''
  name: geo_json
  type: object
provider_name: Agromonitoring
provider_slug: agromonitoring
schema_file: json-schema/agromonitoring-polygoncreaterequest-schema.json
slug: agromonitoring-polygoncreaterequest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.agromonitoring.com/schemas/PolygonCreateRequest.json\",\n  \"title\": \"PolygonCreateRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new field polygon.\",\n  \"required\": [\n    \"name\",\n    \"geo_json\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the field.\",\n      \"example\": \"North Field\"\n    },\n    \"geo_json\": {\n      \"$ref\": \"#/components/schemas/GeoJson\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agromonitoring/refs/heads/main/json-schema/agromonitoring-polygoncreaterequest-schema.json
tags:
- Agriculture
- Satellite Imagery
- Vegetation Indices
- Weather
- Precision Agriculture
- Remote Sensing
title: PolygonCreateRequest
---
