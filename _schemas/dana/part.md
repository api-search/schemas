---
description: A Dana aftermarket part with identifier, descriptive metadata, and compatibility information.
layout: schema
name: Part
properties_list:
- description: The Dana part number.
  name: partNumber
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: category
  type: string
- description: ''
  name: brand
  type: string
- description: ''
  name: make
  type: string
- description: ''
  name: model
  type: string
- description: ''
  name: year
  type: string
- description: ''
  name: specifications
  type: object
- description: ''
  name: images
  type: array
provider_name: Dana
provider_slug: dana
schema_file: json-schema/part.json
slug: part
source_filename: part.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dana/refs/heads/main/json-schema/part.json\",\n  \"title\": \"Part\",\n  \"description\": \"A Dana aftermarket part with identifier, descriptive metadata, and compatibility information.\",\n  \"type\": \"object\",\n  \"required\": [\"partNumber\"],\n  \"properties\": {\n    \"partNumber\": {\"type\": \"string\", \"description\": \"The Dana part number.\"},\n    \"description\": {\"type\": \"string\"},\n    \"category\": {\"type\": \"string\"},\n    \"brand\": {\"type\": \"string\"},\n    \"make\": {\"type\": \"string\"},\n    \"model\": {\"type\": \"string\"},\n    \"year\": {\"type\": \"string\"},\n    \"specifications\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true\n    },\n    \"images\": {\n      \"type\": \"array\",\n      \"items\": {\"type\": \"string\", \"format\": \"uri\"}\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dana/refs/heads/main/json-schema/part.json
tags:
- Aftermarket
- Auto Parts
- Drivetrain
- eCommerce
- Supply Chain
title: Part
---
