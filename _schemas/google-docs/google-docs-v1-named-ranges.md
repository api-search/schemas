---
description: A collection of all the NamedRanges in the document that share a given name.
layout: schema
name: NamedRanges
properties_list:
- description: The name that all the named ranges share.
  name: name
  type: string
- description: The named ranges that share the same name.
  name: namedRanges
  type: array
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-named-ranges-schema.json
slug: google-docs-v1-named-ranges
source_filename: google-docs-v1-named-ranges-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NamedRanges\",\n  \"type\": \"object\",\n  \"description\": \"A collection of all the NamedRanges in the document that share a given name.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name that all the named ranges share.\"\n    },\n    \"namedRanges\": {\n      \"type\": \"array\",\n      \"description\": \"The named ranges that share the same name.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-named-ranges-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: NamedRanges
---
