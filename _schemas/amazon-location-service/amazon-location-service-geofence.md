---
description: Schema representing an Amazon Location Service geofence resource.
layout: schema
name: Amazon Location Service Geofence
properties_list:
- description: The identifier for the geofence.
  name: GeofenceId
  type: string
- description: The geofence geometry.
  name: Geometry
  type: object
- description: The status of the geofence.
  name: Status
  type: string
- description: The timestamp for when the geofence was created.
  name: CreateTime
  type: string
- description: The timestamp for when the geofence was last updated.
  name: UpdateTime
  type: string
- description: Key-value pairs of geofence properties.
  name: GeofenceProperties
  type: object
provider_name: Amazon Location Service
provider_slug: amazon-location-service
schema_file: json-schema/amazon-location-service-geofence-schema.json
slug: amazon-location-service-geofence
source_filename: amazon-location-service-geofence-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://geo.amazonaws.com/schemas/geofence\",\n  \"title\": \"Amazon Location Service Geofence\",\n  \"description\": \"Schema representing an Amazon Location Service geofence resource.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"GeofenceId\",\n    \"Geometry\"\n  ],\n  \"properties\": {\n    \"GeofenceId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier for the geofence.\",\n      \"minLength\": 1,\n      \"maxLength\": 100,\n      \"pattern\": \"^[-._\\\\p{L}\\\\p{N}]+$\"\n    },\n    \"Geometry\": {\n      \"type\": \"object\",\n      \"description\": \"The geofence geometry.\",\n      \"properties\": {\n        \"Polygon\": {\n          \"type\": \"array\",\n          \"description\": \"A polygon geometry represented as an array of linear rings.\",\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\"\
  : \"array\",\n              \"items\": {\n                \"type\": \"number\"\n              },\n              \"minItems\": 2,\n              \"maxItems\": 2\n            },\n            \"minItems\": 4\n          },\n          \"minItems\": 1\n        },\n        \"Circle\": {\n          \"type\": \"object\",\n          \"description\": \"A circle geometry defined by center and radius.\",\n          \"required\": [\n            \"Center\",\n            \"Radius\"\n          ],\n          \"properties\": {\n            \"Center\": {\n              \"type\": \"array\",\n              \"description\": \"The center of the circle as [longitude, latitude].\",\n              \"items\": {\n                \"type\": \"number\"\n              },\n              \"minItems\": 2,\n              \"maxItems\": 2\n            },\n            \"Radius\": {\n              \"type\": \"number\",\n              \"description\": \"The radius of the circle in meters.\",\n              \"minimum\": 0\n   \
  \         }\n          }\n        }\n      }\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the geofence.\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"PENDING\"\n      ]\n    },\n    \"CreateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp for when the geofence was created.\"\n    },\n    \"UpdateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp for when the geofence was last updated.\"\n    },\n    \"GeofenceProperties\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value pairs of geofence properties.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Tag\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"Key\",\n        \"Value\"\n      ],\n      \"properties\": {\n        \"Key\": {\n          \"type\": \"string\"\
  ,\n          \"minLength\": 1,\n          \"maxLength\": 128\n        },\n        \"Value\": {\n          \"type\": \"string\",\n          \"minLength\": 0,\n          \"maxLength\": 256\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-location-service/refs/heads/main/json-schema/amazon-location-service-geofence-schema.json
tags:
- Geocoding
- Geofencing
- Location
- Maps
- Routing
title: Amazon Location Service Geofence
---
