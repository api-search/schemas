---
description: A downloadable resource within a dataset.
layout: schema
name: Resource
properties_list:
- description: Resource identifier.
  name: resourceId
  type: string
- description: Resource type (GeoTIFF, Preview, Metadata, etc.).
  name: type
  type: string
- description: Original filename.
  name: filename
  type: string
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-resource-schema.json
slug: arlula-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://arlula.com/json-schema/resource.json\",\n  \"title\": \"Resource\",\n  \"description\": \"A downloadable resource within a dataset.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceId\": {\n      \"type\": \"string\",\n      \"description\": \"Resource identifier.\",\n      \"examples\": [\n        \"resource-001\"\n      ]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type (GeoTIFF, Preview, Metadata, etc.).\",\n      \"examples\": [\n        \"GeoTIFF\"\n      ]\n    },\n    \"filename\": {\n      \"type\": \"string\",\n      \"description\": \"Original filename.\",\n      \"examples\": [\n        \"imagery.tif\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arlula/refs/heads/main/json-schema/arlula-resource-schema.json
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: Resource
---
