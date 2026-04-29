---
description: A tab within a document. Tabs can contain content and can be nested with child tabs.
layout: schema
name: Tab
properties_list:
- description: The child tabs nested within this tab.
  name: childTabs
  type: array
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-tab-schema.json
slug: google-docs-v1-tab
source_filename: google-docs-v1-tab-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Tab\",\n  \"type\": \"object\",\n  \"description\": \"A tab within a document. Tabs can contain content and can be nested with child tabs.\",\n  \"properties\": {\n    \"childTabs\": {\n      \"type\": \"array\",\n      \"description\": \"The child tabs nested within this tab.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-tab-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: Tab
---
