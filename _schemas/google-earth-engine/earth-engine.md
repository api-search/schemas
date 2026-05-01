---
description: An asset resource from the Google Earth Engine REST API representing an image, image collection, table, or folder.
layout: schema
name: Earth Engine Asset
properties_list:
- description: The type of the asset.
  name: type
  type: string
- description: The name of the asset in the format projects/*/assets/**.
  name: name
  type: string
- description: The asset ID.
  name: id
  type: string
- description: The last time the asset was updated.
  name: updateTime
  type: string
- description: The start time of the data acquisition.
  name: startTime
  type: string
- description: The end time of the data acquisition.
  name: endTime
  type: string
- description: The spatial footprint of the asset as a GeoJSON geometry.
  name: geometry
  type: object
- description: The size of the asset in bytes.
  name: sizeBytes
  type: string
- description: Information about the data bands of an image asset.
  name: bands
  type: array
- description: Key-value properties associated with the asset.
  name: properties
  type: object
- description: The title of the asset.
  name: title
  type: string
- description: A description of the asset.
  name: description
  type: string
provider_name: Google Earth Engine REST
provider_slug: google-earth-engine
schema_file: json-schema/earth-engine.json
slug: earth-engine
source_filename: earth-engine.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-earth-engine/refs/heads/main/json-schema/earth-engine.json\",\n  \"title\": \"Earth Engine Asset\",\n  \"description\": \"An asset resource from the Google Earth Engine REST API representing an image, image collection, table, or folder.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"TYPE_UNSPECIFIED\", \"IMAGE\", \"IMAGE_COLLECTION\", \"TABLE\", \"FOLDER\", \"CLASSIFIER\"],\n      \"description\": \"The type of the asset.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the asset in the format projects/*/assets/**.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The asset ID.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"\
  The last time the asset was updated.\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The start time of the data acquisition.\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The end time of the data acquisition.\"\n    },\n    \"geometry\": {\n      \"type\": \"object\",\n      \"description\": \"The spatial footprint of the asset as a GeoJSON geometry.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\"\n        },\n        \"coordinates\": {\n          \"type\": \"array\"\n        }\n      }\n    },\n    \"sizeBytes\": {\n      \"type\": \"string\",\n      \"description\": \"The size of the asset in bytes.\"\n    },\n    \"bands\": {\n      \"type\": \"array\",\n      \"description\": \"Information about the data bands of an image asset.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\"\
  : {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The band ID.\"\n          },\n          \"dataType\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"precision\": {\n                \"type\": \"string\",\n                \"enum\": [\"PRECISION_UNSPECIFIED\", \"INT\", \"FLOAT\", \"DOUBLE\"]\n              },\n              \"range\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"min\": { \"type\": \"number\" },\n                  \"max\": { \"type\": \"number\" }\n                }\n              }\n            }\n          },\n          \"grid\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"dimensions\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"width\": { \"type\": \"integer\" },\n                  \"height\": { \"type\": \"integer\" }\n                }\n     \
  \         },\n              \"crsCode\": {\n                \"type\": \"string\",\n                \"description\": \"The coordinate reference system code.\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Key-value properties associated with the asset.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the asset.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the asset.\"\n    }\n  },\n  \"required\": [\"type\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-earth-engine/refs/heads/main/json-schema/earth-engine.json
tags:
- Climate
- Earth Observation
- Environmental
- Geospatial
- GIS
- Google
- Remote Sensing
- Satellite Imagery
title: Earth Engine Asset
---
