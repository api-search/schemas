---
description: A specific issue with a rich result item.
layout: schema
name: RichResultsIssue
properties_list:
- description: The type identifier for this issue.
  name: issueType
  type: string
- description: The severity of the issue.
  name: severity
  type: string
- description: A human-readable description of the issue.
  name: issueMessage
  type: string
provider_name: Google Search Console
provider_slug: google-search-console
schema_file: json-schema/google-search-console-rich-results-issue-schema.json
slug: google-search-console-rich-results-issue
source_filename: google-search-console-rich-results-issue-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RichResultsIssue\",\n  \"type\": \"object\",\n  \"description\": \"A specific issue with a rich result item.\",\n  \"properties\": {\n    \"issueType\": {\n      \"type\": \"string\",\n      \"description\": \"The type identifier for this issue.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"The severity of the issue.\"\n    },\n    \"issueMessage\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the issue.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/json-schema/google-search-console-rich-results-issue-schema.json
tags:
- Analytics
- Google
- Search
- SEO
- Webmaster Tools
title: RichResultsIssue
---
