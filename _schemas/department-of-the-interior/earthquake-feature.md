---
description: A single earthquake event represented as a GeoJSON Feature in the USGS earthquake catalog.
layout: schema
name: USGS Earthquake Feature
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: properties
  type: object
- description: ''
  name: geometry
  type: object
provider_name: Department of the Interior
provider_slug: department-of-the-interior
schema_file: json-schema/earthquake-feature-schema.json
slug: earthquake-feature
source_filename: earthquake-feature-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/department-of-the-interior/schemas/earthquake-feature.json\",\n  \"title\": \"USGS Earthquake Feature\",\n  \"description\": \"A single earthquake event represented as a GeoJSON Feature in the USGS earthquake catalog.\",\n  \"type\": \"object\",\n  \"required\": [\"type\", \"id\", \"properties\", \"geometry\"],\n  \"properties\": {\n    \"type\": { \"type\": \"string\", \"const\": \"Feature\" },\n    \"id\": { \"type\": \"string\" },\n    \"properties\": {\n      \"type\": \"object\",\n      \"required\": [\"mag\", \"place\", \"time\"],\n      \"properties\": {\n        \"mag\": { \"type\": \"number\", \"description\": \"Magnitude\" },\n        \"place\": { \"type\": \"string\" },\n        \"time\": { \"type\": \"integer\", \"description\": \"Origin time (Unix ms)\" },\n        \"updated\": { \"type\": \"integer\" },\n        \"tz\": { \"type\": [\"integer\", \"null\"\
  ] },\n        \"url\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"detail\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"felt\": { \"type\": [\"integer\", \"null\"] },\n        \"cdi\": { \"type\": [\"number\", \"null\"] },\n        \"mmi\": { \"type\": [\"number\", \"null\"] },\n        \"alert\": { \"type\": [\"string\", \"null\"], \"enum\": [\"green\", \"yellow\", \"orange\", \"red\", null] },\n        \"status\": { \"type\": \"string\", \"enum\": [\"automatic\", \"reviewed\", \"deleted\"] },\n        \"tsunami\": { \"type\": \"integer\", \"enum\": [0, 1] },\n        \"sig\": { \"type\": \"integer\" },\n        \"magType\": { \"type\": \"string\" },\n        \"type\": { \"type\": \"string\" },\n        \"title\": { \"type\": \"string\" }\n      }\n    },\n    \"geometry\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": { \"type\": \"string\", \"const\": \"Point\" },\n        \"coordinates\": {\n          \"type\": \"array\",\n\
  \          \"items\": { \"type\": \"number\" },\n          \"minItems\": 3,\n          \"maxItems\": 3,\n          \"description\": \"[longitude, latitude, depth_km]\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/json-schema/earthquake-feature-schema.json
tags:
- Federal Government
- Public Lands
- Natural Resources
- Geospatial
title: USGS Earthquake Feature
---
