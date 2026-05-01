---
description: A page within a GitBook space that contains documentation content. Pages can be nested hierarchically and support different types including sheets, groups, and links.
layout: schema
name: GitBook Page
properties_list:
- description: The unique identifier of the page.
  name: id
  type: string
- description: The title of the page.
  name: title
  type: string
- description: The description of the page.
  name: description
  type: string
- description: The type of page.
  name: kind
  type: string
- description: The URL-friendly path of the page.
  name: path
  type: string
- description: Child pages nested under this page.
  name: pages
  type: array
- description: The document content of the page.
  name: document
  type: object
provider_name: GitBook
provider_slug: gitbook
schema_file: json-schema/page.json
slug: page
source_filename: page.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/gitbook/blob/main/json-schema/page.json\",\n  \"title\": \"GitBook Page\",\n  \"description\": \"A page within a GitBook space that contains documentation content. Pages can be nested hierarchically and support different types including sheets, groups, and links.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the page.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the page.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the page.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"sheet\",\n        \"group\",\n        \"link\"\n      ],\n      \"description\": \"The type of page.\"\n    },\n    \"path\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The URL-friendly path of the page.\"\n    },\n    \"pages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"page.json\"\n      },\n      \"description\": \"Child pages nested under this page.\"\n    },\n    \"document\": {\n      \"type\": \"object\",\n      \"description\": \"The document content of the page.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/json-schema/page.json
tags:
- Content
- Documentation
- Experience
- Integrations
- Platform
- SDKs
title: GitBook Page
---
