---
description: Replaces all instances of text matching a criteria with replace text.
layout: schema
name: ReplaceAllTextRequest
properties_list:
- description: The text that will replace the matched text.
  name: replaceText
  type: string
- description: If non-empty, limits the matches to page elements only on the given pages.
  name: pageObjectIds
  type: array
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-replace-all-text-request-schema.json
slug: google-slides-replace-all-text-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReplaceAllTextRequest\",\n  \"type\": \"object\",\n  \"description\": \"Replaces all instances of text matching a criteria with replace text.\\n\",\n  \"properties\": {\n    \"replaceText\": {\n      \"type\": \"string\",\n      \"description\": \"The text that will replace the matched text.\"\n    },\n    \"pageObjectIds\": {\n      \"type\": \"array\",\n      \"description\": \"If non-empty, limits the matches to page elements only on the given pages.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-replace-all-text-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: ReplaceAllTextRequest
---
