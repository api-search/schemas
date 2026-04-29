---
description: ''
layout: schema
name: Building
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: yearBuilt
  type: integer
- description: ''
  name: architect
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: address
  type: string
- description: ''
  name: squareFootage
  type: integer
- description: ''
  name: floors
  type: integer
- description: ''
  name: historicDesignation
  type: string
- description: ''
  name: visitingHours
  type: string
- description: ''
  name: coordinates
  type: object
provider_name: Architect of the Capitol
provider_slug: architect-of-the-capitol
schema_file: json-schema/aoc-data-api-building-schema.json
slug: aoc-data-api-building
source_filename: aoc-data-api-building-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/architect-of-the-capitol/refs/heads/main/json-schema/aoc-data-api-building-schema.json\",\n  \"title\": \"Building\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"yearBuilt\": {\n      \"type\": \"integer\"\n    },\n    \"architect\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"address\": {\n      \"type\": \"string\"\n    },\n    \"squareFootage\": {\n      \"type\": \"integer\"\n    },\n    \"floors\": {\n      \"type\": \"integer\"\n    },\n    \"historicDesignation\": {\n      \"type\": \"string\"\n    },\n    \"visitingHours\": {\n      \"type\": \"string\"\n    },\n    \"coordinates\": {\n      \"type\": \"object\",\n\
  \      \"properties\": {\n        \"latitude\": {\n          \"type\": \"number\"\n        },\n        \"longitude\": {\n          \"type\": \"number\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/architect-of-the-capitol/refs/heads/main/json-schema/aoc-data-api-building-schema.json
tags:
- Federal Government
- Capitol Hill
- Congress
- Historic Preservation
- Government Services
title: Building
---
