---
description: A criteria that matches a specific string of text in the document.
layout: schema
name: SubstringMatchCriteria
properties_list:
- description: The text to search for in the document.
  name: text
  type: string
- description: Indicates whether the search should respect case.
  name: matchCase
  type: boolean
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-substring-match-criteria-schema.json
slug: google-docs-v1-substring-match-criteria
source_filename: google-docs-v1-substring-match-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubstringMatchCriteria\",\n  \"type\": \"object\",\n  \"description\": \"A criteria that matches a specific string of text in the document.\",\n  \"properties\": {\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The text to search for in the document.\"\n    },\n    \"matchCase\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the search should respect case.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-substring-match-criteria-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: SubstringMatchCriteria
---
