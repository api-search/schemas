---
description: LocationModel schema from Avalara API
layout: schema
name: LocationModel
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: companyId
  type: integer
- description: ''
  name: locationCode
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: addressTypeId
  type: string
- description: ''
  name: addressCategoryId
  type: string
- description: ''
  name: line1
  type: string
- description: ''
  name: city
  type: string
- description: ''
  name: region
  type: string
- description: ''
  name: postalCode
  type: string
- description: ''
  name: country
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-location-model-schema.json
slug: avatax-rest-location-model
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-location-model-schema.json\",\n  \"title\": \"LocationModel\",\n  \"description\": \"LocationModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"companyId\": {\n      \"type\": \"integer\"\n    },\n    \"locationCode\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"addressTypeId\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Firm\",\n        \"Location\",\n        \"Salesperson\"\n      ]\n    },\n    \"addressCategoryId\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Storefront\",\n        \"MainOffice\",\n        \"Warehouse\",\n        \"Salesperson\",\n        \"Other\"\n      ]\n    },\n    \"line1\": {\n      \"type\"\
  : \"string\"\n    },\n    \"city\": {\n      \"type\": \"string\"\n    },\n    \"region\": {\n      \"type\": \"string\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\"\n    },\n    \"country\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-location-model-schema.json
tags:
- Taxes
title: LocationModel
---
