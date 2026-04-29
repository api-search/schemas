---
description: A specific mobile usability issue.
layout: schema
name: MobileUsabilityIssue
properties_list:
- description: The type of mobile usability issue.
  name: issueType
  type: string
- description: The severity of the issue.
  name: severity
  type: string
- description: A human-readable description of the issue.
  name: message
  type: string
provider_name: Google Search Console
provider_slug: google-search-console
schema_file: json-schema/google-search-console-mobile-usability-issue-schema.json
slug: google-search-console-mobile-usability-issue
source_filename: google-search-console-mobile-usability-issue-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MobileUsabilityIssue\",\n  \"type\": \"object\",\n  \"description\": \"A specific mobile usability issue.\",\n  \"properties\": {\n    \"issueType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of mobile usability issue.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"The severity of the issue.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the issue.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/json-schema/google-search-console-mobile-usability-issue-schema.json
tags:
- Analytics
- Google
- Search
- SEO
- Webmaster Tools
title: MobileUsabilityIssue
---
