---
description: A product collection in a Shopify store. Collections group products together for merchandising and navigation. Custom collections have manually curated products while smart collections use rules to automatically include products.
layout: schema
name: Shopify Collection
properties_list:
- description: Unique numeric identifier for the collection
  name: id
  type: integer
- description: The name of the collection
  name: title
  type: string
- description: A URL-friendly unique string automatically generated from the title
  name: handle
  type: string
- description: The description of the collection in HTML format
  name: body_html
  type:
  - string
  - 'null'
- description: When the collection was published
  name: published_at
  type:
  - string
  - 'null'
- description: The sort order for products in the collection
  name: sort_order
  type: string
- description: The Liquid template suffix for the collection page
  name: template_suffix
  type:
  - string
  - 'null'
- description: Whether the collection is published to the POS channel
  name: published_scope
  type: string
- description: When the collection was last modified
  name: updated_at
  type: string
- description: The collection image
  name: image
  type:
  - object
  - 'null'
- description: The rules for smart collections that automatically include products
  name: rules
  type: array
- description: Whether products need to match all rules (false) or any rule (true)
  name: disjunctive
  type: boolean
- description: The GraphQL Admin API identifier
  name: admin_graphql_api_id
  type: string
provider_name: Shopify
provider_slug: shopify
schema_file: json-schema/shopify-collection-schema.json
slug: shopify-collection
source_filename: shopify-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://shopify.dev/schemas/collection.json\",\n  \"title\": \"Shopify Collection\",\n  \"description\": \"A product collection in a Shopify store. Collections group products together for merchandising and navigation. Custom collections have manually curated products while smart collections use rules to automatically include products.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier for the collection\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the collection\"\n    },\n    \"handle\": {\n      \"type\": \"string\",\n      \"description\": \"A URL-friendly unique string automatically generated from the title\"\n    },\n    \"body_html\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The description of the collection in HTML format\"\
  \n    },\n    \"published_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"When the collection was published\"\n    },\n    \"sort_order\": {\n      \"type\": \"string\",\n      \"description\": \"The sort order for products in the collection\",\n      \"enum\": [\n        \"alpha-asc\",\n        \"alpha-desc\",\n        \"best-selling\",\n        \"created\",\n        \"created-desc\",\n        \"manual\",\n        \"price-asc\",\n        \"price-desc\"\n      ]\n    },\n    \"template_suffix\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The Liquid template suffix for the collection page\"\n    },\n    \"published_scope\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the collection is published to the POS channel\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the collection was last modified\"\n    },\n\
  \    \"image\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The collection image\",\n      \"properties\": {\n        \"src\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The image URL\"\n        },\n        \"alt\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Alt text for the image\"\n        },\n        \"width\": {\n          \"type\": \"integer\"\n        },\n        \"height\": {\n          \"type\": \"integer\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    },\n    \"rules\": {\n      \"type\": \"array\",\n      \"description\": \"The rules for smart collections that automatically include products\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"column\": {\n            \"type\": \"string\",\n            \"description\": \"The property to match\
  \ against\",\n            \"enum\": [\"title\", \"type\", \"vendor\", \"variant_price\", \"tag\", \"variant_compare_at_price\", \"variant_weight\", \"variant_inventory\", \"variant_title\"]\n          },\n          \"relation\": {\n            \"type\": \"string\",\n            \"description\": \"The comparison operator\",\n            \"enum\": [\"equals\", \"not_equals\", \"starts_with\", \"ends_with\", \"contains\", \"not_contains\", \"greater_than\", \"less_than\"]\n          },\n          \"condition\": {\n            \"type\": \"string\",\n            \"description\": \"The value to compare against\"\n          }\n        }\n      }\n    },\n    \"disjunctive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether products need to match all rules (false) or any rule (true)\"\n    },\n    \"admin_graphql_api_id\": {\n      \"type\": \"string\",\n      \"description\": \"The GraphQL Admin API identifier\"\n    }\n  },\n  \"required\": [\"id\", \"title\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/shopify/refs/heads/main/json-schema/shopify-collection-schema.json
tags:
- Commerce
- Ecommerce
- Payments
- Retail
- Shopping Cart
- T1
title: Shopify Collection
---
