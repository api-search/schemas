---
description: An Amazon Location Service map resource.
layout: schema
name: MapResource
properties_list:
- description: The name of the map resource.
  name: MapName
  type: string
- description: The Amazon Resource Name (ARN) for the map resource.
  name: MapArn
  type: string
- description: Specifies the map data provider.
  name: DataSource
  type: string
- description: An optional description for the map resource.
  name: Description
  type: string
- description: The timestamp for when the map resource was created.
  name: CreateTime
  type: string
- description: The timestamp for when the map resource was last updated.
  name: UpdateTime
  type: string
provider_name: Amazon Location Service
provider_slug: amazon-location-service
schema_file: json-schema/amazon-location-service-map-schema.json
slug: amazon-location-service-map
source_filename: amazon-location-service-map-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-location-service/refs/heads/main/json-schema/amazon-location-service-map-schema.json\",\n  \"title\": \"MapResource\",\n  \"description\": \"An Amazon Location Service map resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MapName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the map resource.\",\n      \"example\": \"my-map\"\n    },\n    \"MapArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) for the map resource.\"\n    },\n    \"DataSource\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the map data provider.\",\n      \"example\": \"HERE\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"An optional description for the map resource.\"\n    },\n    \"CreateTime\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The timestamp for when the map resource was created.\",\n      \"format\": \"date-time\"\n    },\n    \"UpdateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The timestamp for when the map resource was last updated.\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-location-service/refs/heads/main/json-schema/amazon-location-service-map-schema.json
tags:
- Geocoding
- Geofencing
- Location
- Maps
- Routing
title: MapResource
---
