---
description: A Zesty.io content model defines the structure and schema for content items within an instance, including fields and their types.
layout: schema
name: Zesty Content Model
properties_list:
- description: The Zesty Universal Identifier for the content model.
  name: ZUID
  type: string
- description: The name of the content model.
  name: name
  type: string
- description: The display label for the content model.
  name: label
  type: string
- description: The type of the content model.
  name: type
  type: string
- description: A description of the content model.
  name: description
  type: string
- description: The parent content model ZUID for nested models.
  name: parentZUID
  type: string
- description: Whether the model appears in navigation.
  name: listed
  type: boolean
- description: Timestamp when the content model was created.
  name: createdAt
  type: string
- description: Timestamp when the content model was last updated.
  name: updatedAt
  type: string
provider_name: Zesty
provider_slug: zesty
schema_file: json-schema/content-model.json
slug: content-model
source_filename: content-model.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/zesty/blob/main/json-schema/content-model.json\",\n  \"title\": \"Zesty Content Model\",\n  \"description\": \"A Zesty.io content model defines the structure and schema for content items within an instance, including fields and their types.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ZUID\": {\n      \"type\": \"string\",\n      \"description\": \"The Zesty Universal Identifier for the content model.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the content model.\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"The display label for the content model.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"templateset\", \"pageset\", \"dataset\", \"headless\"],\n      \"description\": \"The type of the content model.\"\n    },\n    \"description\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"A description of the content model.\"\n    },\n    \"parentZUID\": {\n      \"type\": \"string\",\n      \"description\": \"The parent content model ZUID for nested models.\"\n    },\n    \"listed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the model appears in navigation.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the content model was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the content model was last updated.\"\n    }\n  },\n  \"required\": [\"ZUID\", \"name\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/json-schema/content-model.json
tags:
- CMS
- Composable
- Content Management
- Headless CMS
- Media
title: Zesty Content Model
---
