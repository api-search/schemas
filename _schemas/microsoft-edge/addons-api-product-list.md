---
description: Paginated list of extension products in the Microsoft Edge Add-ons store
layout: schema
name: ProductList
properties_list:
- description: Array of products
  name: value
  type: array
- description: Total number of products
  name: totalCount
  type: integer
provider_name: Microsoft Edge
provider_slug: microsoft-edge
schema_file: json-schema/addons-api-product-list-schema.json
slug: addons-api-product-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/json-schema/addons-api-product-list-schema.json\",\n  \"title\": \"ProductList\",\n  \"description\": \"Paginated list of extension products in the Microsoft Edge Add-ons store\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"description\": \"Array of products\",\n      \"items\": {\n        \"$ref\": \"addons-api-product-schema.json\"\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of products\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/json-schema/addons-api-product-list-schema.json
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
title: ProductList
---
