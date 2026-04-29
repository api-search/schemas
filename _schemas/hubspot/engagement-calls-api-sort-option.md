---
description: Sort option for search results
layout: schema
name: SortOption
properties_list:
- description: The property to sort by
  name: propertyName
  type: string
- description: Sort direction
  name: direction
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/engagement-calls-api-sort-option-schema.json
slug: engagement-calls-api-sort-option
source_filename: engagement-calls-api-sort-option-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-calls-api-sort-option-schema.json\",\n  \"title\": \"SortOption\",\n  \"description\": \"Sort option for search results\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"propertyName\": {\n      \"type\": \"string\",\n      \"description\": \"The property to sort by\",\n      \"example\": \"hs_timestamp\"\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ASCENDING\",\n        \"DESCENDING\"\n      ],\n      \"description\": \"Sort direction\",\n      \"default\": \"DESCENDING\",\n      \"example\": \"DESCENDING\"\n    }\n  },\n  \"required\": [\n    \"propertyName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-calls-api-sort-option-schema.json
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
title: SortOption
---
