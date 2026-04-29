---
description: ''
layout: schema
name: Address
properties_list:
- description: The street address of the property.
  name: street
  type: string
- description: The city where the property is located.
  name: city
  type: string
- description: The state or province where the property is located.
  name: state
  type: string
- description: The postal or ZIP code.
  name: zip_code
  type: string
- description: The ISO 3166-1 alpha-2 country code.
  name: country
  type: string
- description: The latitude coordinate of the property.
  name: latitude
  type: number
- description: The longitude coordinate of the property.
  name: longitude
  type: number
provider_name: airbnb
provider_slug: airbnb
schema_file: json-schema/airbnb-address-schema.json
slug: airbnb-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-address-schema.json\",\n  \"title\": \"Address\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"street\": {\n      \"type\": \"string\",\n      \"description\": \"The street address of the property.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"The city where the property is located.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The state or province where the property is located.\"\n    },\n    \"zip_code\": {\n      \"type\": \"string\",\n      \"description\": \"The postal or ZIP code.\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 3166-1 alpha-2 country code.\",\n      \"pattern\": \"^[A-Z]{2}$\"\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\
  ,\n      \"description\": \"The latitude coordinate of the property.\",\n      \"minimum\": -90,\n      \"maximum\": 90\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The longitude coordinate of the property.\",\n      \"minimum\": -180,\n      \"maximum\": 180\n    }\n  },\n  \"required\": [\n    \"street\",\n    \"city\",\n    \"country\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-address-schema.json
tags: []
title: Address
---
