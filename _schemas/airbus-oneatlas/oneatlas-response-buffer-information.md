---
description: GeoJSon feature describing a buffer
layout: schema
name: responseBufferInformation
properties_list:
- description: ''
  name: geometry
  type: object
- description: ''
  name: properties
  type: object
- description: the type of the GeoJSon object
  name: type
  type: string
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-response-buffer-information-schema.json
slug: oneatlas-response-buffer-information
source_filename: oneatlas-response-buffer-information-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-response-buffer-information-schema.json\",\n  \"title\": \"responseBufferInformation\",\n  \"type\": \"object\",\n  \"description\": \"GeoJSon feature describing a buffer\",\n  \"properties\": {\n    \"geometry\": {\n      \"$ref\": \"#/components/schemas/GeojsonGeometry\"\n    },\n    \"properties\": {\n      \"properties\": {\n        \"aoi\": {\n          \"$ref\": \"#/components/schemas/bbox\"\n        },\n        \"bands\": {\n          \"items\": {\n            \"$ref\": \"#/components/schemas/band\"\n          },\n          \"minItems\": 1,\n          \"type\": \"array\"\n        },\n        \"format\": {\n          \"description\": \"the MIME type of the buffer\",\n          \"enum\": [\n            \"image/jp2\",\n            \"image/jpeg\",\n            \"image/png\",\n            \"\
  application/octet-stream\"\n          ],\n          \"type\": \"string\"\n        },\n        \"height\": {\n          \"description\": \"height of the buffer\",\n          \"example\": 500,\n          \"format\": \"integer\",\n          \"maximum\": 5000,\n          \"minimum\": 1,\n          \"type\": \"number\"\n        },\n        \"imageID\": {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        \"interleave\": {\n          \"description\": \"the interleave type of the buffer\",\n          \"enum\": [\n            \"band\",\n            \"line\",\n            \"pixel\"\n          ],\n          \"type\": \"string\"\n        },\n        \"nbBands\": {\n          \"description\": \"the number of bands of the buffer\",\n          \"example\": 1,\n          \"format\": \"integer\",\n          \"minimum\": 1,\n          \"type\": \"number\"\n        },\n        \"noDataValue\": {\n          \"description\": \"the value of a pixel that does not correspond to a real data\"\
  ,\n          \"format\": \"integer\",\n          \"minimum\": 0,\n          \"type\": \"number\"\n        },\n        \"pixelType\": {\n          \"description\": \"the type of pixel of the buffer\",\n          \"example\": \"UInt16\",\n          \"type\": \"string\"\n        },\n        \"processingLevel\": {\n          \"example\": \"processingLevel\",\n          \"type\": \"string\"\n        },\n        \"radiometricProcessing\": {\n          \"example\": \"reflectance\",\n          \"type\": \"string\"\n        },\n        \"roi\": {\n          \"$ref\": \"#/components/schemas/bbox\"\n        },\n        \"spectralProcessing\": {\n          \"example\": \"P\",\n          \"type\": \"string\"\n        },\n        \"step\": {\n          \"$ref\": \"#/components/schemas/step\"\n        },\n        \"width\": {\n          \"description\": \"width of the buffer\",\n          \"example\": 500,\n          \"format\": \"integer\",\n          \"maximum\": 5000,\n          \"minimum\": 1,\n\
  \          \"type\": \"number\"\n        }\n      },\n      \"type\": \"object\"\n    },\n    \"type\": {\n      \"description\": \"the type of the GeoJSon object\",\n      \"enum\": [\n        \"Feature\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-response-buffer-information-schema.json
tags:
- Imagery
- Satellites
title: responseBufferInformation
---
