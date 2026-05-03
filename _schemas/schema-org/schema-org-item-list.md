---
description: A list of items of any sort, for example, Top 10 Restaurants, Recommended Products, or a list of music tracks.
layout: schema
name: Schema.org ItemList
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The name of the list.
  name: name
  type: string
- description: A description of the list.
  name: description
  type: string
- description: URL of the list.
  name: url
  type: string
- description: The items in the list.
  name: itemListElement
  type: array
- description: Type of ordering.
  name: itemListOrder
  type: string
- description: The number of items in an ItemList.
  name: numberOfItems
  type: integer
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-item-list-schema.json
slug: schema-org-item-list
source_filename: schema-org-item-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/item-list.json\",\n  \"title\": \"Schema.org ItemList\",\n  \"description\": \"A list of items of any sort, for example, Top 10 Restaurants, Recommended Products, or a list of music tracks.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"itemListElement\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The Schema.org type.\",\n      \"enum\": [\"ItemList\", \"BreadcrumbList\", \"HowToSection\", \"HowToStep\", \"OfferCatalog\"]\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the list.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the list.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"uri\",\n      \"description\": \"URL of the list.\"\n    },\n    \"itemListElement\": {\n      \"type\": \"array\",\n      \"description\": \"The items in the list.\",\n      \"items\": {\n        \"oneOf\": [\n          { \"$ref\": \"#/$defs/ListItem\" },\n          { \"type\": \"object\" },\n          { \"type\": \"string\" }\n        ]\n      }\n    },\n    \"itemListOrder\": {\n      \"type\": \"string\",\n      \"enum\": [\"ItemListOrderAscending\", \"ItemListOrderDescending\", \"ItemListUnordered\"],\n      \"description\": \"Type of ordering.\"\n    },\n    \"numberOfItems\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of items in an ItemList.\"\n    }\n  },\n  \"$defs\": {\n    \"ListItem\": {\n      \"type\": \"object\",\n      \"description\": \"An item in a list.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"ListItem\" },\n        \"position\": { \"type\": \"integer\", \"description\": \"The position of an item\
  \ in a series.\" },\n        \"name\": { \"type\": \"string\", \"description\": \"The name of the item.\" },\n        \"url\": { \"type\": \"string\", \"format\": \"uri\", \"description\": \"URL of the item.\" },\n        \"item\": {\n          \"type\": \"object\",\n          \"description\": \"The item represented by this list item.\",\n          \"properties\": {\n            \"@type\": { \"type\": \"string\" },\n            \"name\": { \"type\": \"string\" },\n            \"url\": { \"type\": \"string\", \"format\": \"uri\" }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-item-list-schema.json
tags:
- Schema.org
- Structured Data
- Linked Data
- JSON-LD
- Vocabulary
- SEO
- Web Standards
- RDF
- Ontology
title: Schema.org ItemList
---
