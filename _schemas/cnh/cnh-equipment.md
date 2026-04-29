---
description: Equipment record returned by the CNH FieldOps API for agronomic and construction machinery (Case IH, New Holland, STEYR, Case CE, New Holland Construction).
layout: schema
name: CNH FieldOps Equipment
properties_list:
- description: FieldOps-assigned unique identifier for the vehicle.
  name: vehicleId
  type: string
- description: CNH Industrial brand.
  name: brand
  type: string
- description: Model name as registered with FieldOps.
  name: model
  type: string
- description: Manufacturer serial number / VIN-equivalent.
  name: serialNumber
  type: string
- description: Model year.
  name: year
  type: integer
- description: Vehicle category.
  name: vehicleType
  type: string
- description: Friendly display name set by the operator.
  name: displayName
  type: string
provider_name: CNH
provider_slug: cnh
schema_file: json-schema/cnh-equipment-schema.json
slug: cnh-equipment
source_filename: cnh-equipment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cnh/main/json-schema/cnh-equipment-schema.json\",\n  \"title\": \"CNH FieldOps Equipment\",\n  \"description\": \"Equipment record returned by the CNH FieldOps API for agronomic and construction machinery (Case IH, New Holland, STEYR, Case CE, New Holland Construction).\",\n  \"type\": \"object\",\n  \"required\": [\"vehicleId\", \"brand\", \"model\"],\n  \"properties\": {\n    \"vehicleId\": {\n      \"type\": \"string\",\n      \"description\": \"FieldOps-assigned unique identifier for the vehicle.\"\n    },\n    \"brand\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CASE_IH\",\n        \"NEW_HOLLAND\",\n        \"STEYR\",\n        \"CASE_CE\",\n        \"NEW_HOLLAND_CONSTRUCTION\"\n      ],\n      \"description\": \"CNH Industrial brand.\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Model\
  \ name as registered with FieldOps.\"\n    },\n    \"serialNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Manufacturer serial number / VIN-equivalent.\"\n    },\n    \"year\": {\n      \"type\": \"integer\",\n      \"minimum\": 1980,\n      \"maximum\": 2100,\n      \"description\": \"Model year.\"\n    },\n    \"vehicleType\": {\n      \"type\": \"string\",\n      \"enum\": [\"TRACTOR\", \"COMBINE\", \"SPRAYER\", \"CONSTRUCTION\"],\n      \"description\": \"Vehicle category.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Friendly display name set by the operator.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cnh/refs/heads/main/json-schema/cnh-equipment-schema.json
tags:
- Agriculture
- Construction
- Telematics
- Equipment
- FieldOps
title: CNH FieldOps Equipment
---
