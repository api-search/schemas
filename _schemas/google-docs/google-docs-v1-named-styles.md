---
description: The named styles defined in the document. Paragraphs in the document can inherit their text and paragraph styles from these named styles.
layout: schema
name: NamedStyles
properties_list:
- description: The named styles.
  name: styles
  type: array
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-named-styles-schema.json
slug: google-docs-v1-named-styles
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NamedStyles\",\n  \"type\": \"object\",\n  \"description\": \"The named styles defined in the document. Paragraphs in the document can inherit their text and paragraph styles from these named styles.\",\n  \"properties\": {\n    \"styles\": {\n      \"type\": \"array\",\n      \"description\": \"The named styles.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-named-styles-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: NamedStyles
---
