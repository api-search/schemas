---
description: An NPS-managed unit (national park, monument, recreation area, historic site, etc.).
layout: schema
name: National Park
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: fullName
  type: string
- description: Four-letter NPS park code
  name: parkCode
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: latitude
  type: string
- description: ''
  name: longitude
  type: string
- description: Comma-separated two-letter state codes
  name: states
  type: string
- description: e.g. National Park, National Monument, National Historical Park
  name: designation
  type: string
- description: ''
  name: directionsInfo
  type: string
- description: ''
  name: weatherInfo
  type: string
- description: ''
  name: operatingHours
  type: array
- description: ''
  name: entranceFees
  type: array
- description: ''
  name: activities
  type: array
- description: ''
  name: topics
  type: array
- description: ''
  name: images
  type: array
provider_name: Department of the Interior
provider_slug: department-of-the-interior
schema_file: json-schema/nps-park-schema.json
slug: nps-park
source_filename: nps-park-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/department-of-the-interior/schemas/park.json\",\n  \"title\": \"National Park\",\n  \"description\": \"An NPS-managed unit (national park, monument, recreation area, historic site, etc.).\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"parkCode\", \"fullName\"],\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"format\": \"uuid\" },\n    \"url\": { \"type\": \"string\", \"format\": \"uri\" },\n    \"fullName\": { \"type\": \"string\" },\n    \"parkCode\": { \"type\": \"string\", \"minLength\": 4, \"maxLength\": 4, \"description\": \"Four-letter NPS park code\" },\n    \"description\": { \"type\": \"string\" },\n    \"latitude\": { \"type\": \"string\" },\n    \"longitude\": { \"type\": \"string\" },\n    \"states\": { \"type\": \"string\", \"description\": \"Comma-separated two-letter state codes\" },\n    \"designation\": { \"type\": \"string\", \"\
  description\": \"e.g. National Park, National Monument, National Historical Park\" },\n    \"directionsInfo\": { \"type\": \"string\" },\n    \"weatherInfo\": { \"type\": \"string\" },\n    \"operatingHours\": { \"type\": \"array\", \"items\": { \"type\": \"object\" } },\n    \"entranceFees\": { \"type\": \"array\", \"items\": { \"type\": \"object\" } },\n    \"activities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": { \"id\": { \"type\": \"string\" }, \"name\": { \"type\": \"string\" } }\n      }\n    },\n    \"topics\": { \"type\": \"array\", \"items\": { \"type\": \"object\" } },\n    \"images\": { \"type\": \"array\", \"items\": { \"type\": \"object\" } }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/json-schema/nps-park-schema.json
tags:
- Federal Government
- Public Lands
- Natural Resources
- Geospatial
title: National Park
---
