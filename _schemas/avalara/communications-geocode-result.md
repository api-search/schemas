---
description: GeocodeResult schema from Avalara API
layout: schema
name: GeocodeResult
properties_list:
- description: ''
  name: ref
  type: string
- description: ''
  name: cass
  type: object
- description: Census block group
  name: cBlk
  type: string
- description: Census tract
  name: cTrc
  type: string
- description: Error message if geocoding failed
  name: err
  type: string
- description: Whether geocoding was successful
  name: geo
  type: boolean
- description: ''
  name: lat
  type: number
- description: ''
  name: long
  type: number
- description: PCode for the determined jurisdiction
  name: pcd
  type: integer
- description: FIPS code
  name: fips
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-geocode-result-schema.json
slug: communications-geocode-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-geocode-result-schema.json\",\n  \"title\": \"GeocodeResult\",\n  \"description\": \"GeocodeResult schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ref\": {\n      \"type\": \"string\"\n    },\n    \"cass\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"addr\": {\n          \"type\": \"string\"\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"st\": {\n          \"type\": \"string\"\n        },\n        \"zip\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"cBlk\": {\n      \"type\": \"string\",\n      \"description\": \"Census block group\"\n    },\n    \"cTrc\": {\n      \"type\": \"string\",\n      \"description\": \"Census tract\"\n    },\n    \"err\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Error message if geocoding failed\"\n    },\n    \"geo\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether geocoding was successful\"\n    },\n    \"lat\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"long\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"pcd\": {\n      \"type\": \"integer\",\n      \"description\": \"PCode for the determined jurisdiction\"\n    },\n    \"fips\": {\n      \"type\": \"string\",\n      \"description\": \"FIPS code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-geocode-result-schema.json
tags:
- Taxes
title: GeocodeResult
---
