---
description: ''
layout: schema
name: dem
properties_list:
- description: ''
  name: key
  type: object
- description: Defines the digital elevation model, i refers to the aoi's id (To be filled only if processing_level = ortho)
  name: value
  type: object
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-dem-schema.json
slug: oneatlas-dem
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-dem-schema.json\",\n  \"title\": \"dem\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"enum\": [\n        \"dem_i\"\n      ]\n    },\n    \"value\": {\n      \"description\": \"Defines the digital elevation model, i refers to the aoi's id (To be filled only if processing_level = ortho)\",\n      \"enum\": [\n        \"best_available\",\n        \"FLAT_DEM_WITH_GTOPO30_WAT\",\n        \"FLAT_DEM_WITH_WAT\",\n        \"GTOPO30\",\n        \"MIXEDDEM\",\n        \"PAS-DEM\",\n        \"PAS-DEM_IVV\",\n        \"REF3D-DEM\",\n        \"REF3D-DEM_IVV\",\n        \"SRTMV4\",\n        \"SRTMV4_IVV\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-dem-schema.json
tags:
- Imagery
- Satellites
title: dem
---
