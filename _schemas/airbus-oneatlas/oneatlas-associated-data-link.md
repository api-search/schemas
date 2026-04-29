---
description: ''
layout: schema
name: AssociatedDataLink
properties_list:
- description: ''
  name: content
  type: string
- description: ''
  name: mimeType
  type: string
- description: ''
  name: path
  type: string
- description: ''
  name: title
  type: string
- description: See [Get associated data](#/paths/~1api~1v1~1items~1{catalogItemId}~1images~1{imageId}~1associatedData~1{associatedDataType}~1data/get)
  name: url
  type: string
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-associated-data-link-schema.json
slug: oneatlas-associated-data-link
source_filename: oneatlas-associated-data-link-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-associated-data-link-schema.json\",\n  \"title\": \"AssociatedDataLink\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"example\": \"GML MASK\",\n      \"type\": \"string\"\n    },\n    \"mimeType\": {\n      \"example\": \"application/gml+xml\",\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"example\": \"MASKS/ROI_SPOT6_P_201602011017034_SEN_2551123101_MSK.GML\",\n      \"type\": \"string\"\n    },\n    \"title\": {\n      \"example\": \"LUT Mask\",\n      \"type\": \"string\"\n    },\n    \"url\": {\n      \"description\": \"See [Get associated data](#/paths/~1api~1v1~1items~1{catalogItemId}~1images~1{imageId}~1associatedData~1{associatedDataType}~1data/get)\",\n      \"example\": \"https://view.foundation.api.oneatlas.com/api/v1/items/f494e323-e132-4aac-aad2-5123176a6800/images/5a277ab0-5315-4042-a676-267152d71e17/associatedData/LUT/data\"\
  ,\n      \"format\": \"url\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-associated-data-link-schema.json
tags:
- Imagery
- Satellites
title: AssociatedDataLink
---
