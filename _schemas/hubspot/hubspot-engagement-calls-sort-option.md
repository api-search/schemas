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
schema_file: json-schema/hubspot-engagement-calls-sort-option-schema.json
slug: hubspot-engagement-calls-sort-option
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Sort option for search results\",\n  \"properties\": {\n    \"propertyName\": {\n      \"type\": \"string\",\n      \"description\": \"The property to sort by\",\n      \"example\": \"hs_timestamp\"\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"description\": \"Sort direction\",\n      \"example\": \"DESCENDING\",\n      \"enum\": [\n        \"ASCENDING\",\n        \"DESCENDING\"\n      ]\n    }\n  },\n  \"required\": [\n    \"propertyName\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SortOption\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-calls-sort-option-schema.json
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
