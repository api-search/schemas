---
description: Vehicle information for car insurance estimates
layout: schema
name: Vehicle
properties_list:
- description: Vehicle manufacturer
  name: make
  type: string
- description: Vehicle model name
  name: model
  type: string
- description: Year of manufacture
  name: year
  type: integer
- description: Vehicle registration number
  name: registration
  type: string
provider_name: Allianz
provider_slug: allianz-docs
schema_file: json-schema/api-connect-vehicle-schema.json
slug: api-connect-vehicle
source_filename: api-connect-vehicle-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-vehicle-schema.json\",\n  \"title\": \"Vehicle\",\n  \"description\": \"Vehicle information for car insurance estimates\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"make\": {\n      \"type\": \"string\",\n      \"description\": \"Vehicle manufacturer\",\n      \"example\": \"Toyota\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Vehicle model name\",\n      \"example\": \"Camry\"\n    },\n    \"year\": {\n      \"type\": \"integer\",\n      \"description\": \"Year of manufacture\",\n      \"example\": 2022\n    },\n    \"registration\": {\n      \"type\": \"string\",\n      \"description\": \"Vehicle registration number\",\n      \"example\": \"ABC123\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-vehicle-schema.json
tags:
- Financial Services
- Insurance
- Asset Management
title: Vehicle
---
