---
description: Service schema from Aramark Marko API
layout: schema
name: Service
properties_list:
- description: Service identifier
  name: id
  type: string
- description: Service type
  name: type
  type: string
- description: Location identifier
  name: locationId
  type: string
- description: Service status
  name: status
  type: string
- description: Service name
  name: name
  type: string
provider_name: Aramark
provider_slug: aramark
schema_file: json-schema/marko-api-service-schema.json
slug: marko-api-service
source_filename: marko-api-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Service identifier\",\n      \"example\": \"SVC-001\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Service type\",\n      \"enum\": [\n        \"FOOD_SERVICE\",\n        \"FACILITIES\",\n        \"UNIFORM\",\n        \"RETAIL\"\n      ],\n      \"example\": \"FOOD_SERVICE\"\n    },\n    \"locationId\": {\n      \"type\": \"string\",\n      \"description\": \"Location identifier\",\n      \"example\": \"LOC-001\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Service status\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"INACTIVE\",\n        \"SUSPENDED\"\n      ],\n      \"example\": \"ACTIVE\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Service name\",\n      \"example\": \"Campus Dining\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/json-schema/marko-api-service-schema.json\",\n  \"title\": \"Service\",\n  \"description\": \"Service schema from Aramark Marko API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/json-schema/marko-api-service-schema.json
tags:
- Food Services
- Facilities Management
- Uniform Services
- Data Platform
- Fortune 500
title: Service
---
