---
description: The content of a tab in a document, containing the body and associated document-level properties.
layout: schema
name: DocumentTab
properties_list:
- description: The headers in this tab, keyed by header ID.
  name: headers
  type: object
- description: The footers in this tab, keyed by footer ID.
  name: footers
  type: object
- description: The footnotes in this tab, keyed by footnote ID.
  name: footnotes
  type: object
- description: The lists in this tab, keyed by list ID.
  name: lists
  type: object
- description: The named ranges in this tab, keyed by name.
  name: namedRanges
  type: object
- description: The inline objects in this tab, keyed by object ID.
  name: inlineObjects
  type: object
- description: The positioned objects in this tab, keyed by object ID.
  name: positionedObjects
  type: object
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-document-tab-schema.json
slug: google-docs-v1-document-tab
source_filename: google-docs-v1-document-tab-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DocumentTab\",\n  \"type\": \"object\",\n  \"description\": \"The content of a tab in a document, containing the body and associated document-level properties.\",\n  \"properties\": {\n    \"headers\": {\n      \"type\": \"object\",\n      \"description\": \"The headers in this tab, keyed by header ID.\"\n    },\n    \"footers\": {\n      \"type\": \"object\",\n      \"description\": \"The footers in this tab, keyed by footer ID.\"\n    },\n    \"footnotes\": {\n      \"type\": \"object\",\n      \"description\": \"The footnotes in this tab, keyed by footnote ID.\"\n    },\n    \"lists\": {\n      \"type\": \"object\",\n      \"description\": \"The lists in this tab, keyed by list ID.\"\n    },\n    \"namedRanges\": {\n      \"type\": \"object\",\n      \"description\": \"The named ranges in this tab, keyed by name.\"\n    },\n    \"inlineObjects\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"The inline objects in this tab, keyed by object ID.\"\n    },\n    \"positionedObjects\": {\n      \"type\": \"object\",\n      \"description\": \"The positioned objects in this tab, keyed by object ID.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-document-tab-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: DocumentTab
---
