---
description: A Webflow Collection Item representing a single entry in a CMS collection, as returned by the Webflow Data API v2. Each item includes system metadata, status flags, and content fields stored in fieldData.
layout: schema
name: Webflow Collection Item
properties_list:
- description: Unique identifier for the Item.
  name: id
  type: string
- description: Identifier for the locale of the CMS item.
  name: cmsLocaleId
  type: string
- description: The date the item was last published.
  name: lastPublished
  type:
  - string
  - 'null'
- description: The date the item was last updated.
  name: lastUpdated
  type: string
- description: The date the item was created.
  name: createdOn
  type: string
- description: Boolean determining if the Item is set to archived.
  name: isArchived
  type: boolean
- description: Boolean determining if the Item is set to draft.
  name: isDraft
  type: boolean
- description: An object containing the item's content fields. Every item requires a name and slug. Additional fields are dynamic and match the collection's schema definition.
  name: fieldData
  type: object
provider_name: Webflow
provider_slug: webflow
schema_file: json-schema/webflow-collection-item-schema.json
slug: webflow-collection-item
source_filename: webflow-collection-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.webflow.com/schemas/collection-item.json\",\n  \"title\": \"Webflow Collection Item\",\n  \"description\": \"A Webflow Collection Item representing a single entry in a CMS collection, as returned by the Webflow Data API v2. Each item includes system metadata, status flags, and content fields stored in fieldData.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"fieldData\",\n    \"lastPublished\",\n    \"lastUpdated\",\n    \"createdOn\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"description\": \"Unique identifier for the Item.\",\n      \"examples\": [\"580e64008c9a982ac9b8b754\"]\n    },\n    \"cmsLocaleId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier for the locale of the CMS item.\",\n      \"examples\": [\"653ad57de882f528b32e810e\"]\n    },\n    \"lastPublished\": {\n   \
  \   \"type\": [\"string\", \"null\"],\n      \"readOnly\": true,\n      \"description\": \"The date the item was last published.\",\n      \"examples\": [\"2023-03-17T18:47:35.560Z\"]\n    },\n    \"lastUpdated\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"description\": \"The date the item was last updated.\",\n      \"examples\": [\"2023-03-17T18:47:35.560Z\"]\n    },\n    \"createdOn\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"description\": \"The date the item was created.\",\n      \"examples\": [\"2023-03-17T18:47:35.560Z\"]\n    },\n    \"isArchived\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Boolean determining if the Item is set to archived.\"\n    },\n    \"isDraft\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Boolean determining if the Item is set to draft.\"\n    },\n    \"fieldData\": {\n      \"type\": \"object\",\n      \"description\":\
  \ \"An object containing the item's content fields. Every item requires a name and slug. Additional fields are dynamic and match the collection's schema definition.\",\n      \"required\": [\n        \"name\",\n        \"slug\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the Item.\",\n          \"examples\": [\"The Hitchhiker's Guide to the Galaxy\"]\n        },\n        \"slug\": {\n          \"type\": \"string\",\n          \"description\": \"URL structure of the Item in your site. Updates to an item slug will break all links referencing the old slug.\",\n          \"examples\": [\"hitchhikers-guide-to-the-galaxy\"]\n        }\n      },\n      \"additionalProperties\": true\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/json-schema/webflow-collection-item-schema.json
tags:
- CMS
- Ecommerce
- No-Code
- Web Development
title: Webflow Collection Item
---
