---
description: A criteria that specifies in which tabs a request executes.
layout: schema
name: TabsCriteria
properties_list:
- description: The list of tab IDs in which the request executes. An empty list signifies that the request executes in all tabs.
  name: tabIds
  type: array
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-tabs-criteria-schema.json
slug: google-docs-v1-tabs-criteria
source_filename: google-docs-v1-tabs-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TabsCriteria\",\n  \"type\": \"object\",\n  \"description\": \"A criteria that specifies in which tabs a request executes.\",\n  \"properties\": {\n    \"tabIds\": {\n      \"type\": \"array\",\n      \"description\": \"The list of tab IDs in which the request executes. An empty list signifies that the request executes in all tabs.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-tabs-criteria-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: TabsCriteria
---
