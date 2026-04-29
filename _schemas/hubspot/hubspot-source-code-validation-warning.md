---
description: A validation warning
layout: schema
name: ValidationWarning
properties_list:
- description: Warning description
  name: message
  type: string
- description: Line number where the warning occurred
  name: line
  type: integer
- description: Suggested fix
  name: suggestion
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-source-code-validation-warning-schema.json
slug: hubspot-source-code-validation-warning
source_filename: hubspot-source-code-validation-warning-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A validation warning\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Warning description\",\n      \"example\": \"Deprecated function 'blog_recent_posts' used\"\n    },\n    \"line\": {\n      \"type\": \"integer\",\n      \"description\": \"Line number where the warning occurred\",\n      \"example\": 28\n    },\n    \"suggestion\": {\n      \"type\": \"string\",\n      \"description\": \"Suggested fix\",\n      \"example\": \"Use 'blog_posts' function instead\"\n    }\n  },\n  \"required\": [\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ValidationWarning\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-source-code-validation-warning-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: ValidationWarning
---
