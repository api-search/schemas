---
description: PropertyInput schema from ARGUS Enterprise API
layout: schema
name: PropertyInput
properties_list:
- description: Property name
  name: name
  type: string
- description: ''
  name: propertyType
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: address
  type: object
- description: ''
  name: grossArea
  type: number
- description: ''
  name: netLeasableArea
  type: number
- description: ''
  name: yearBuilt
  type: integer
- description: ''
  name: numberOfUnits
  type: integer
- description: ''
  name: purchasePrice
  type: number
- description: ''
  name: purchaseDate
  type: string
- description: ''
  name: portfolioId
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-property-input-schema.json
slug: argus-enterprise-property-input
source_filename: argus-enterprise-property-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-property-input-schema.json\",\n  \"title\": \"PropertyInput\",\n  \"description\": \"PropertyInput schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Property name\"\n    },\n    \"propertyType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Office\",\n        \"Retail\",\n        \"Industrial\",\n        \"Multifamily\",\n        \"Mixed-Use\",\n        \"Hotel\",\n        \"Land\",\n        \"Other\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Active\",\n        \"Pending\",\n        \"Archived\"\n      ],\n      \"default\": \"Active\"\n    },\n    \"address\": {\n      \"$ref\": \"#/components/schemas/Address\"\n\
  \    },\n    \"grossArea\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"netLeasableArea\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"yearBuilt\": {\n      \"type\": \"integer\"\n    },\n    \"numberOfUnits\": {\n      \"type\": \"integer\"\n    },\n    \"purchasePrice\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"purchaseDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"portfolioId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"propertyType\",\n    \"address\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-property-input-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: PropertyInput
---
