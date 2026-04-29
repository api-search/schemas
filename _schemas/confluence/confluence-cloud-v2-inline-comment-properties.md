---
description: Properties specific to inline comments.
layout: schema
name: InlineCommentProperties
properties_list:
- description: The selected text that this inline comment is anchored to.
  name: textSelection
  type: string
- description: The match index of the text selection, if the same text appears multiple times.
  name: textSelectionMatchCount
  type: integer
provider_name: Confluence
provider_slug: confluence
schema_file: json-schema/confluence-cloud-v2-inline-comment-properties-schema.json
slug: confluence-cloud-v2-inline-comment-properties
source_filename: confluence-cloud-v2-inline-comment-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InlineCommentProperties\",\n  \"type\": \"object\",\n  \"description\": \"Properties specific to inline comments.\",\n  \"properties\": {\n    \"textSelection\": {\n      \"type\": \"string\",\n      \"description\": \"The selected text that this inline comment is anchored to.\"\n    },\n    \"textSelectionMatchCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The match index of the text selection, if the same text appears multiple times.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/json-schema/confluence-cloud-v2-inline-comment-properties-schema.json
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
title: InlineCommentProperties
---
