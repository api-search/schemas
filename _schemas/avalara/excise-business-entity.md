---
description: BusinessEntity schema from Avalara API
layout: schema
name: BusinessEntity
properties_list:
- description: ''
  name: entityId
  type: string
- description: ''
  name: entityName
  type: string
- description: ''
  name: entityType
  type: string
- description: Federal EIN
  name: federalIdNumber
  type: string
- description: ''
  name: address
  type: object
- description: ''
  name: isActive
  type: boolean
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/excise-business-entity-schema.json
slug: excise-business-entity
source_filename: excise-business-entity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-business-entity-schema.json\",\n  \"title\": \"BusinessEntity\",\n  \"description\": \"BusinessEntity schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entityId\": {\n      \"type\": \"string\"\n    },\n    \"entityName\": {\n      \"type\": \"string\"\n    },\n    \"entityType\": {\n      \"type\": \"string\"\n    },\n    \"federalIdNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Federal EIN\"\n    },\n    \"address\": {\n      \"$ref\": \"#/components/schemas/ExciseAddress\"\n    },\n    \"isActive\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-business-entity-schema.json
tags:
- Taxes
title: BusinessEntity
---
