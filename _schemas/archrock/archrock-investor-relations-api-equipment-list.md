---
description: ''
layout: schema
name: EquipmentList
properties_list:
- description: ''
  name: total
  type: integer
- description: ''
  name: offset
  type: integer
- description: ''
  name: limit
  type: integer
- description: ''
  name: equipment
  type: array
provider_name: Archrock
provider_slug: archrock
schema_file: json-schema/archrock-investor-relations-api-equipment-list-schema.json
slug: archrock-investor-relations-api-equipment-list
source_filename: archrock-investor-relations-api-equipment-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archrock/refs/heads/main/json-schema/archrock-investor-relations-api-equipment-list-schema.json\",\n  \"title\": \"EquipmentList\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    },\n    \"equipment\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {},\n          \"unitNumber\": {},\n          \"horsepowerRating\": {},\n          \"engineType\": {},\n          \"compressionType\": {},\n          \"status\": {},\n          \"location\": {},\n          \"customer\": {},\n          \"deploymentDate\": {}\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archrock/refs/heads/main/json-schema/archrock-investor-relations-api-equipment-list-schema.json
tags:
- Natural Gas
- Compression Services
- Oil And Gas
- Energy
- Industrial
- 'NYSE: AROC'
title: EquipmentList
---
