---
description: Metadata about a single available Salesforce REST API version on this instance.
layout: schema
name: ApiVersion
properties_list:
- description: The API version number (e.g., "63.0").
  name: version
  type: string
- description: Descriptive label for this API version (e.g., "Winter '25").
  name: label
  type: string
- description: The REST endpoint URL for this specific API version on the current instance.
  name: url
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-rest-api-version-schema.json
slug: salesforce-rest-api-version
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Metadata about a single available Salesforce REST API version on this instance.\\n\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The API version number (e.g., \\\"63.0\\\").\",\n      \"example\": \"example_value\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Descriptive label for this API version (e.g., \\\"Winter '25\\\").\",\n      \"example\": \"Example Title\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The REST endpoint URL for this specific API version on the current instance.\\n\",\n      \"format\": \"uri\",\n      \"example\": \"https://www.example.com\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApiVersion\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-rest-api-version-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: ApiVersion
---
