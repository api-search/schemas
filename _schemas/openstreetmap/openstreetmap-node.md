---
description: An OSM node — the fundamental building block of OSM map data, representing a geographic point
layout: schema
name: OpenStreetMap Node
properties_list:
- description: ''
  name: type
  type: string
- description: OSM node ID (positive integer)
  name: id
  type: integer
- description: Latitude in decimal degrees (WGS84)
  name: lat
  type: number
- description: Longitude in decimal degrees (WGS84)
  name: lon
  type: number
- description: Key-value metadata tags (e.g., name, amenity, highway)
  name: tags
  type: object
- description: Edit version number (incremented on each modification)
  name: version
  type: integer
- description: ID of the changeset that last modified this node
  name: changeset
  type: integer
- description: UTC timestamp of the last modification
  name: timestamp
  type: string
- description: Username of the last editor
  name: user
  type: string
- description: User ID of the last editor
  name: uid
  type: integer
- description: False if the node was deleted in this version
  name: visible
  type: boolean
provider_name: OpenStreetMap
provider_slug: openstreetmap
schema_file: json-schema/openstreetmap-node-schema.json
slug: openstreetmap-node
source_filename: openstreetmap-node-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/json-schema/openstreetmap-node-schema.json\",\n  \"title\": \"OpenStreetMap Node\",\n  \"description\": \"An OSM node — the fundamental building block of OSM map data, representing a geographic point\",\n  \"type\": \"object\",\n  \"required\": [\"type\", \"id\", \"lat\", \"lon\"],\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"node\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"minimum\": 1,\n      \"description\": \"OSM node ID (positive integer)\"\n    },\n    \"lat\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"minimum\": -90,\n      \"maximum\": 90,\n      \"description\": \"Latitude in decimal degrees (WGS84)\"\n    },\n    \"lon\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n  \
  \    \"minimum\": -180,\n      \"maximum\": 180,\n      \"description\": \"Longitude in decimal degrees (WGS84)\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Key-value metadata tags (e.g., name, amenity, highway)\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"Edit version number (incremented on each modification)\"\n    },\n    \"changeset\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"ID of the changeset that last modified this node\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"UTC timestamp of the last modification\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the last editor\"\n    },\n    \"uid\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"User ID of the last editor\"\n    },\n    \"visible\": {\n      \"type\": \"boolean\",\n      \"description\": \"False if the node was deleted in this version\"\n    }\n  },\n  \"$defs\": {\n    \"Way\": {\n      \"title\": \"OSM Way\",\n      \"description\": \"An OSM way — an ordered list of nodes forming a line or closed polygon\",\n      \"type\": \"object\",\n      \"required\": [\"type\", \"id\", \"nodes\"],\n      \"properties\": {\n        \"type\": { \"type\": \"string\", \"const\": \"way\" },\n        \"id\": { \"type\": \"integer\", \"format\": \"int64\" },\n        \"nodes\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"integer\", \"format\": \"int64\" },\n          \"minItems\": 2,\n          \"maxItems\": 2000,\n          \"description\": \"Ordered list of node IDs forming the way\"\n        },\n        \"tags\": {\n          \"type\": \"object\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        },\n        \"version\": {\
  \ \"type\": \"integer\" },\n        \"changeset\": { \"type\": \"integer\", \"format\": \"int64\" },\n        \"timestamp\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"user\": { \"type\": \"string\" },\n        \"uid\": { \"type\": \"integer\" },\n        \"visible\": { \"type\": \"boolean\" }\n      }\n    },\n    \"Relation\": {\n      \"title\": \"OSM Relation\",\n      \"description\": \"An OSM relation — groups nodes, ways, and other relations with typed membership roles\",\n      \"type\": \"object\",\n      \"required\": [\"type\", \"id\", \"members\"],\n      \"properties\": {\n        \"type\": { \"type\": \"string\", \"const\": \"relation\" },\n        \"id\": { \"type\": \"integer\", \"format\": \"int64\" },\n        \"members\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"required\": [\"type\", \"ref\"],\n            \"properties\": {\n              \"type\": { \"type\": \"string\", \"enum\"\
  : [\"node\", \"way\", \"relation\"] },\n              \"ref\": { \"type\": \"integer\", \"format\": \"int64\" },\n              \"role\": { \"type\": \"string\", \"description\": \"Semantic role (e.g., outer, inner, stop, platform)\" }\n            }\n          }\n        },\n        \"tags\": {\n          \"type\": \"object\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        },\n        \"version\": { \"type\": \"integer\" },\n        \"changeset\": { \"type\": \"integer\", \"format\": \"int64\" },\n        \"timestamp\": { \"type\": \"string\", \"format\": \"date-time\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/json-schema/openstreetmap-node-schema.json
tags:
- Geospatial
- Mapping
- Open Data
- Geocoding
- Editing
title: OpenStreetMap Node
---
