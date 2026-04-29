---
description: ''
layout: schema
name: GeoJSONFeatureCollection
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: features
  type: array
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-asset-registry-geojsonfeaturecollection-schema.json
slug: agstack-asset-registry-geojsonfeaturecollection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/GeoJSONFeatureCollection.json\",\n  \"title\": \"GeoJSONFeatureCollection\",\n  \"type\": \"object\",\n  \"required\": [\n    \"type\",\n    \"features\"\n  ],\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"FeatureCollection\"\n      ]\n    },\n    \"features\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\n          \"geometry\"\n        ],\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"example\": \"Feature\"\n          },\n          \"geometry\": {\n            \"type\": \"object\",\n            \"required\": [\n              \"type\",\n              \"coordinates\"\n            ],\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"enum\"\
  : [\n                  \"Point\"\n                ]\n              },\n              \"coordinates\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"number\"\n                },\n                \"example\": [\n                  75.78209,\n                  30.90706\n                ]\n              }\n            }\n          },\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"Optional properties like s2_index\",\n            \"properties\": {\n              \"s2_index\": {\n                \"type\": \"string\",\n                \"example\": \"8,13\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-asset-registry-geojsonfeaturecollection-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: GeoJSONFeatureCollection
---
