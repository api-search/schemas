---
description: The schema for a Fumadocs meta.json file placed in a documentation directory. Meta files configure the folder's display title, the ordered list of pages shown in the sidebar, default open and collapsible state, and whether the folder acts as a navigation root. When a meta.json is absent, Fumadocs generates default navigation from the file system order.
layout: schema
name: Fumadocs Meta
properties_list:
- description: The display name for this documentation folder as shown in the sidebar navigation. Overrides the directory name.
  name: title
  type: string
- description: 'An ordered list of page slugs or folder names controlling the sequence in which items appear in the sidebar. Items not listed appear after listed items in filesystem order. Use ''...'' as a placeholder '
  name: pages
  type: array
- description: A short description of this documentation section displayed as supplementary text in navigation.
  name: description
  type: string
- description: When true, this folder acts as a secondary navigation root. Activating any page within this folder causes the sidebar to display only this folder's contents, hiding the broader navigation tree.
  name: root
  type: boolean
- description: When true, this folder section is expanded by default in the sidebar regardless of whether a child page is currently active.
  name: defaultOpen
  type: boolean
- description: Controls whether users can collapse this folder section in the sidebar. Defaults to true. Set to false to keep the folder always expanded.
  name: collapsible
  type: boolean
- description: Icon identifier or inline SVG content displayed alongside the folder title in sidebar navigation.
  name: icon
  type: string
provider_name: Fumadocs
provider_slug: fumadocs
schema_file: json-schema/fumadocs-meta-schema.json
slug: fumadocs-meta
source_filename: fumadocs-meta-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://fumadocs.dev/schemas/meta.json\",\n  \"title\": \"Fumadocs Meta\",\n  \"description\": \"The schema for a Fumadocs meta.json file placed in a documentation directory. Meta files configure the folder's display title, the ordered list of pages shown in the sidebar, default open and collapsible state, and whether the folder acts as a navigation root. When a meta.json is absent, Fumadocs generates default navigation from the file system order.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The display name for this documentation folder as shown in the sidebar navigation. Overrides the directory name.\",\n      \"example\": \"API Reference\"\n    },\n    \"pages\": {\n      \"type\": \"array\",\n      \"description\": \"An ordered list of page slugs or folder names controlling the sequence in which items appear in the\
  \ sidebar. Items not listed appear after listed items in filesystem order. Use '...' as a placeholder to insert remaining unlisted pages at that position.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"Page slug (filename without extension), subdirectory name, or '...' placeholder.\"\n      },\n      \"example\": [\"index\", \"getting-started\", \"...\", \"advanced\"]\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A short description of this documentation section displayed as supplementary text in navigation.\"\n    },\n    \"root\": {\n      \"type\": \"boolean\",\n      \"description\": \"When true, this folder acts as a secondary navigation root. Activating any page within this folder causes the sidebar to display only this folder's contents, hiding the broader navigation tree.\"\n    },\n    \"defaultOpen\": {\n      \"type\": \"boolean\",\n      \"description\": \"When true, this folder section is expanded\
  \ by default in the sidebar regardless of whether a child page is currently active.\"\n    },\n    \"collapsible\": {\n      \"type\": \"boolean\",\n      \"description\": \"Controls whether users can collapse this folder section in the sidebar. Defaults to true. Set to false to keep the folder always expanded.\"\n    },\n    \"icon\": {\n      \"type\": \"string\",\n      \"description\": \"Icon identifier or inline SVG content displayed alongside the folder title in sidebar navigation.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fumadocs/refs/heads/main/json-schema/fumadocs-meta-schema.json
tags:
- Documentation
- Framework
- Next.js
- React
title: Fumadocs Meta
---
