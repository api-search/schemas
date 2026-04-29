---
description: A criteria that matches a specific string of text in a shape or table.
layout: schema
name: SubstringMatchCriteria
properties_list:
- description: The text to search for in the shape or table.
  name: text
  type: string
- description: Indicates whether the search should respect case. True by default.
  name: matchCase
  type: boolean
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-substring-match-criteria-schema.json
slug: google-slides-substring-match-criteria
source_filename: google-slides-substring-match-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubstringMatchCriteria\",\n  \"type\": \"object\",\n  \"description\": \"A criteria that matches a specific string of text in a shape or table.\\n\",\n  \"properties\": {\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The text to search for in the shape or table.\"\n    },\n    \"matchCase\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the search should respect case. True by default.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-substring-match-criteria-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: SubstringMatchCriteria
---
