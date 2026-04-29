---
description: A Best Buy store location with operational details.
layout: schema
name: Store
properties_list:
- description: Unique store identifier.
  name: storeId
  type: integer
- description: Short store name.
  name: name
  type: string
- description: Full store name including address.
  name: longName
  type: string
- description: Street address of the store.
  name: address
  type: string
- description: Secondary address line (suite, building, etc.).
  name: address2
  type: string
- description: City where the store is located.
  name: city
  type: string
- description: Two-letter US state abbreviation.
  name: state
  type: string
- description: US postal code.
  name: zipcode
  type: string
- description: Store phone number.
  name: phone
  type: string
- description: Store latitude coordinate.
  name: lat
  type: number
- description: Store longitude coordinate.
  name: lng
  type: number
- description: Distance from the search location in miles (when area query is used).
  name: distance
  type: number
- description: Store format type.
  name: storeType
  type: string
- description: Store hours summary.
  name: hours
  type: string
- description: GMT offset for the store's timezone.
  name: gmtOffset
  type: integer
- description: Services offered at this store location.
  name: services
  type: array
provider_name: Best Buy
provider_slug: best-buy
schema_file: json-schema/stores-api-store-schema.json
slug: stores-api-store
source_filename: stores-api-store-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/json-schema/stores-api-store-schema.json\",\n  \"title\": \"Store\",\n  \"description\": \"A Best Buy store location with operational details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"storeId\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique store identifier.\",\n      \"example\": 281\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Short store name.\",\n      \"example\": \"Best Buy - San Francisco\"\n    },\n    \"longName\": {\n      \"type\": \"string\",\n      \"description\": \"Full store name including address.\",\n      \"example\": \"Best Buy San Francisco - 1717 Harrison St\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Street address of the store.\",\n      \"example\": \"1717 Harrison St\"\n    },\n    \"address2\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Secondary address line (suite, building, etc.).\",\n      \"example\": \"\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City where the store is located.\",\n      \"example\": \"San Francisco\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Two-letter US state abbreviation.\",\n      \"example\": \"CA\"\n    },\n    \"zipcode\": {\n      \"type\": \"string\",\n      \"description\": \"US postal code.\",\n      \"example\": \"94103\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Store phone number.\",\n      \"example\": \"415-626-9682\"\n    },\n    \"lat\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Store latitude coordinate.\",\n      \"example\": 37.771\n    },\n    \"lng\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Store longitude\
  \ coordinate.\",\n      \"example\": -122.411\n    },\n    \"distance\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Distance from the search location in miles (when area query is used).\",\n      \"example\": 0.8\n    },\n    \"storeType\": {\n      \"type\": \"string\",\n      \"description\": \"Store format type.\",\n      \"enum\": [\n        \"Big Box\",\n        \"Express Kiosk\",\n        \"Warehouse Sale\",\n        \"Outlet Center\",\n        \"PAC Standalone\"\n      ],\n      \"example\": \"Big Box\"\n    },\n    \"hours\": {\n      \"type\": \"string\",\n      \"description\": \"Store hours summary.\",\n      \"example\": \"Mon-Sat 10am-8pm, Sun 11am-7pm\"\n    },\n    \"gmtOffset\": {\n      \"type\": \"integer\",\n      \"description\": \"GMT offset for the store's timezone.\",\n      \"example\": -8\n    },\n    \"services\": {\n      \"type\": \"array\",\n      \"description\": \"Services offered at this store location.\",\n \
  \     \"items\": {\n        \"$ref\": \"#/components/schemas/StoreService\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/json-schema/stores-api-store-schema.json
tags:
- Retail
- Consumer Electronics
- E-Commerce
- Products
- Stores
title: Store
---
