---
description: A commerce item representing a product in a purchase or shopping cart event tracked through the Iterable Commerce API. Commerce items capture product details for revenue attribution and abandoned cart campaigns.
layout: schema
name: Iterable Commerce Item
properties_list:
- description: Unique item identifier or product ID
  name: id
  type: string
- description: Stock keeping unit identifier
  name: sku
  type: string
- description: Display name of the product
  name: name
  type: string
- description: Product description text
  name: description
  type: string
- description: Product categories for classification and filtering
  name: categories
  type: array
- description: Unit price of the item
  name: price
  type: number
- description: Number of units purchased or in cart
  name: quantity
  type: integer
- description: URL of the product image
  name: imageUrl
  type: string
- description: URL of the product page
  name: url
  type: string
- description: Custom data fields associated with the item
  name: dataFields
  type: object
provider_name: Iterable
provider_slug: iterable
schema_file: json-schema/iterable-commerce-item-schema.json
slug: iterable-commerce-item
source_filename: iterable-commerce-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.api-evangelist.com/schemas/iterable/commerce-item.json\",\n  \"title\": \"Iterable Commerce Item\",\n  \"description\": \"A commerce item representing a product in a purchase or shopping cart event tracked through the Iterable Commerce API. Commerce items capture product details for revenue attribution and abandoned cart campaigns.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"price\", \"quantity\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"description\": \"Unique item identifier or product ID\"\n    },\n    \"sku\": {\n      \"type\": \"string\",\n      \"description\": \"Stock keeping unit identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"description\": \"Display name of the product\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n  \
  \    \"description\": \"Product description text\"\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"description\": \"Product categories for classification and filtering\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Unit price of the item\"\n    },\n    \"quantity\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"Number of units purchased or in cart\"\n    },\n    \"imageUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the product image\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the product page\"\n    },\n    \"dataFields\": {\n      \"type\": \"object\",\n      \"description\": \"Custom data fields associated with the item\",\n      \"additionalProperties\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/json-schema/iterable-commerce-item-schema.json
tags:
- Cross-Channel Messaging
- Customer Engagement
- Email
- Marketing Automation
- Push Notifications
- SMS
title: Iterable Commerce Item
---
