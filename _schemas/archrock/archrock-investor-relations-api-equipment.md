---
description: ''
layout: schema
name: Equipment
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: unitNumber
  type: string
- description: ''
  name: horsepowerRating
  type: integer
- description: ''
  name: engineType
  type: string
- description: ''
  name: compressionType
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: location
  type: string
- description: ''
  name: customer
  type: string
- description: ''
  name: deploymentDate
  type: string
provider_name: Archrock
provider_slug: archrock
schema_file: json-schema/archrock-investor-relations-api-equipment-schema.json
slug: archrock-investor-relations-api-equipment
source_filename: archrock-investor-relations-api-equipment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archrock/refs/heads/main/json-schema/archrock-investor-relations-api-equipment-schema.json\",\n  \"title\": \"Equipment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"unitNumber\": {\n      \"type\": \"string\"\n    },\n    \"horsepowerRating\": {\n      \"type\": \"integer\"\n    },\n    \"engineType\": {\n      \"type\": \"string\"\n    },\n    \"compressionType\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"active\",\n        \"idle\",\n        \"maintenance\"\n      ]\n    },\n    \"location\": {\n      \"type\": \"string\"\n    },\n    \"customer\": {\n      \"type\": \"string\"\n    },\n    \"deploymentDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archrock/refs/heads/main/json-schema/archrock-investor-relations-api-equipment-schema.json
tags:
- Natural Gas
- Compression Services
- Oil And Gas
- Energy
- Industrial
- 'NYSE: AROC'
title: Equipment
---
