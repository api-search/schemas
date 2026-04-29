---
description: An extension product in the Microsoft Edge Add-ons store
layout: schema
name: Product
properties_list:
- description: Product identifier
  name: id
  type: string
- description: Extension name
  name: name
  type: string
- description: Extension description
  name: description
  type: string
- description: Product publishing status
  name: status
  type: string
- description: Current published version
  name: version
  type: string
- description: Last update timestamp
  name: lastUpdatedUtc
  type: string
- description: Store category
  name: category
  type: string
provider_name: Microsoft Edge
provider_slug: microsoft-edge
schema_file: json-schema/addons-api-product-schema.json
slug: addons-api-product
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/json-schema/addons-api-product-schema.json\",\n  \"title\": \"Product\",\n  \"description\": \"An extension product in the Microsoft Edge Add-ons store\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Product identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Extension name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Extension description\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Product publishing status\",\n      \"enum\": [\"Draft\", \"InReview\", \"Published\", \"Unpublished\", \"Rejected\"]\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Current published version\"\n    },\n    \"\
  lastUpdatedUtc\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last update timestamp\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Store category\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/json-schema/addons-api-product-schema.json
tags:
- Browser
- Chromium
- Developer Tools
- Edge
- Extensions
- Microsoft
- Progressive Web Apps
- Web Development
- WebView
title: Product
---
