---
description: 'The act of searching for an object. Related actions: FindAction.'
layout: schema
name: Schema.org SearchAction
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: Indicates a target EntryPoint for an Action.
  name: target
  type: object
- description: A sub property of object. The query used on this action (e.g., required name=search_term_string).
  name: query-input
  type: string
- description: The query string.
  name: query
  type: string
- description: Indicates the current disposition of the Action.
  name: actionStatus
  type: string
- description: The result produced in the action.
  name: result
  type: object
- description: The name of the action.
  name: name
  type: string
- description: A description of the action.
  name: description
  type: string
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-search-action-schema.json
slug: schema-org-search-action
source_filename: schema-org-search-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/search-action.json\",\n  \"title\": \"Schema.org SearchAction\",\n  \"description\": \"The act of searching for an object. Related actions: FindAction.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"const\": \"SearchAction\",\n      \"description\": \"The Schema.org type.\"\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"target\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"$ref\": \"#/$defs/EntryPoint\" }\n      ],\n      \"description\": \"Indicates a target EntryPoint for an Action.\"\n    },\n    \"query-input\": {\n      \"type\": \"string\",\n      \"description\": \"A sub property of object. The query used on this action (e.g., required name=search_term_string).\"\
  \n    },\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"The query string.\"\n    },\n    \"actionStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\"ActiveActionStatus\", \"CompletedActionStatus\", \"FailedActionStatus\", \"PotentialActionStatus\"],\n      \"description\": \"Indicates the current disposition of the Action.\"\n    },\n    \"result\": {\n      \"type\": \"object\",\n      \"description\": \"The result produced in the action.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the action.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the action.\"\n    }\n  },\n  \"$defs\": {\n    \"EntryPoint\": {\n      \"type\": \"object\",\n      \"description\": \"An entry point for a URL-addressable action.\",\n      \"properties\"\
  : {\n        \"@type\": { \"type\": \"string\", \"const\": \"EntryPoint\" },\n        \"urlTemplate\": { \"type\": \"string\", \"description\": \"A URL template for the action.\" },\n        \"actionPlatform\": {\n          \"oneOf\": [\n            { \"type\": \"string\" },\n            { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n          ],\n          \"description\": \"The high level platform(s) where the Action can be performed.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-search-action-schema.json
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
title: Schema.org SearchAction
---
