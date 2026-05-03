---
description: A BreadcrumbList is an ItemList consisting of a chain of linked Web pages, typically described using at least their URL and their name, and typically ending with the current page.
layout: schema
name: Schema.org BreadcrumbList
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The list of breadcrumb items.
  name: itemListElement
  type: array
- description: The name of the breadcrumb list.
  name: name
  type: string
- description: A description of the breadcrumb list.
  name: description
  type: string
- description: The number of items in the breadcrumb list.
  name: numberOfItems
  type: integer
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-breadcrumb-list-schema.json
slug: schema-org-breadcrumb-list
source_filename: schema-org-breadcrumb-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/breadcrumb-list.json\",\n  \"title\": \"Schema.org BreadcrumbList\",\n  \"description\": \"A BreadcrumbList is an ItemList consisting of a chain of linked Web pages, typically described using at least their URL and their name, and typically ending with the current page.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"itemListElement\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"const\": \"BreadcrumbList\",\n      \"description\": \"The Schema.org type.\"\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"itemListElement\": {\n      \"type\": \"array\",\n      \"description\": \"The list of breadcrumb items.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ListItem\"\n      }\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"\
  The name of the breadcrumb list.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the breadcrumb list.\"\n    },\n    \"numberOfItems\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of items in the breadcrumb list.\"\n    }\n  },\n  \"$defs\": {\n    \"ListItem\": {\n      \"type\": \"object\",\n      \"description\": \"An item in a breadcrumb list.\",\n      \"required\": [\"@type\", \"position\"],\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"ListItem\" },\n        \"position\": { \"type\": \"integer\", \"description\": \"The position of an item in a series.\" },\n        \"name\": { \"type\": \"string\", \"description\": \"The name of the item.\" },\n        \"item\": {\n          \"oneOf\": [\n            { \"type\": \"string\", \"format\": \"uri\" },\n            { \"type\": \"object\", \"properties\": { \"@type\": { \"type\": \"string\" }, \"@id\": { \"type\": \"string\"\
  , \"format\": \"uri\" }, \"name\": { \"type\": \"string\" } } }\n          ],\n          \"description\": \"The item represented by this list item.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-breadcrumb-list-schema.json
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
title: Schema.org BreadcrumbList
---
