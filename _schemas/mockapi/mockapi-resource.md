---
description: Schema describing a mockAPI.io resource definition. Captures the resource name, fields, relationships, and seed configuration so a portable definition can be replayed in mockAPI or another mock platform.
layout: schema
name: mockAPI Resource
properties_list:
- description: ''
  name: id
  type: string
- description: Resource name. Used to derive REST paths (e.g., /users).
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: fields
  type: array
- description: ''
  name: relationships
  type: array
- description: Number of records to generate when the resource is provisioned.
  name: seedCount
  type: integer
- description: ''
  name: endpoints
  type: array
provider_name: mockAPI
provider_slug: mockapi
schema_file: json-schema/mockapi-resource-schema.json
slug: mockapi-resource
source_filename: mockapi-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/mockapi/main/json-schema/mockapi-resource-schema.json\",\n  \"title\": \"mockAPI Resource\",\n  \"description\": \"Schema describing a mockAPI.io resource definition. Captures the resource name, fields, relationships, and seed configuration so a portable definition can be replayed in mockAPI or another mock platform.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"fields\"],\n  \"properties\": {\n    \"id\": { \"type\": \"string\" },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Resource name. Used to derive REST paths (e.g., /users).\"\n    },\n    \"description\": { \"type\": \"string\" },\n    \"fields\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"name\", \"type\"],\n        \"properties\": {\n          \"name\": { \"type\": \"string\" },\n   \
  \       \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\"string\", \"integer\", \"number\", \"boolean\", \"object\", \"array\", \"datetime\", \"uuid\", \"faker\"]\n          },\n          \"faker\": {\n            \"type\": \"string\",\n            \"description\": \"Faker.js expression used to generate seed values (e.g., name.firstName).\"\n          },\n          \"required\": { \"type\": \"boolean\", \"default\": false },\n          \"default\": {},\n          \"description\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"relationships\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"resource\", \"type\"],\n        \"properties\": {\n          \"resource\": { \"type\": \"string\" },\n          \"type\": { \"type\": \"string\", \"enum\": [\"hasOne\", \"hasMany\", \"belongsTo\"] }\n        }\n      }\n    },\n    \"seedCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n   \
  \   \"description\": \"Number of records to generate when the resource is provisioned.\"\n    },\n    \"endpoints\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"method\", \"path\"],\n        \"properties\": {\n          \"method\": { \"type\": \"string\", \"enum\": [\"GET\", \"POST\", \"PUT\", \"PATCH\", \"DELETE\"] },\n          \"path\": { \"type\": \"string\" },\n          \"responseCode\": { \"type\": \"integer\", \"minimum\": 100, \"maximum\": 599 },\n          \"delayMs\": { \"type\": \"integer\", \"minimum\": 0 }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mockapi/refs/heads/main/json-schema/mockapi-resource-schema.json
tags:
- API Mocking
- CRUD
- Mock Server
- Mocking
- Platform
- Prototyping
- REST
- Testing
title: mockAPI Resource
---
