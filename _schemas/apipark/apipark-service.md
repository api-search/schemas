---
description: Schema representing an API service published in the APIPark developer portal
layout: schema
name: APIPark Service
properties_list:
- description: Unique identifier of the service
  name: id
  type: string
- description: Name of the API service
  name: name
  type: string
- description: Description of the service
  name: description
  type: string
- description: Team that owns this service
  name: teamId
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: tags
  type: array
- description: ''
  name: createdAt
  type: string
provider_name: APIPark
provider_slug: apipark
schema_file: json-schema/apipark-service-schema.json
slug: apipark-service
source_filename: apipark-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apipark/main/json-schema/apipark-service-schema.json\",\n  \"title\": \"APIPark Service\",\n  \"description\": \"Schema representing an API service published in the APIPark developer portal\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Unique identifier of the service\" },\n    \"name\": { \"type\": \"string\", \"description\": \"Name of the API service\" },\n    \"description\": { \"type\": \"string\", \"description\": \"Description of the service\" },\n    \"teamId\": { \"type\": \"string\", \"description\": \"Team that owns this service\" },\n    \"status\": { \"type\": \"string\", \"enum\": [\"draft\", \"published\", \"deprecated\"] },\n    \"tags\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n    \"createdAt\": { \"type\": \"string\", \"format\": \"date-time\" }\n\
  \  },\n  \"required\": [\"id\", \"name\", \"teamId\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apipark/refs/heads/main/json-schema/apipark-service-schema.json
tags:
- AI Gateway
- API Gateway
- API Management
- Developer Portal
- LLM
- Open Source
title: APIPark Service
---
