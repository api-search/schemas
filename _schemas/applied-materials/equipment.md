---
description: Semiconductor manufacturing equipment managed by Applied Materials
layout: schema
name: Equipment
properties_list:
- description: Unique equipment identifier
  name: equipmentId
  type: string
- description: Equipment serial number
  name: serialNumber
  type: string
- description: Equipment model name
  name: model
  type: string
- description: Equipment type (CVD, PVD, CMP, Etch, etc.)
  name: type
  type: string
- description: Current operational status
  name: status
  type: string
- description: Fab location where equipment is installed
  name: location
  type: string
- description: Date equipment was installed
  name: installDate
  type: string
- description: Date of last scheduled maintenance
  name: lastMaintenanceDate
  type: string
provider_name: Applied Materials
provider_slug: applied-materials
schema_file: json-schema/equipment-schema.json
slug: equipment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/applied-materials/main/json-schema/equipment-schema.json\",\n  \"title\": \"Equipment\",\n  \"description\": \"Semiconductor manufacturing equipment managed by Applied Materials\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"equipmentId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique equipment identifier\"\n    },\n    \"serialNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Equipment serial number\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Equipment model name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Equipment type (CVD, PVD, CMP, Etch, etc.)\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"operational\",\n        \"maintenance\",\n        \"idle\",\n        \"error\"\n      ],\n \
  \     \"description\": \"Current operational status\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Fab location where equipment is installed\"\n    },\n    \"installDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date equipment was installed\"\n    },\n    \"lastMaintenanceDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of last scheduled maintenance\"\n    }\n  },\n  \"required\": [\n    \"equipmentId\",\n    \"serialNumber\",\n    \"model\",\n    \"type\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/applied-materials/refs/heads/main/json-schema/equipment-schema.json
tags:
- Semiconductor
- Manufacturing
- Equipment
- Fab Operations
- Materials Engineering
title: Equipment
---
