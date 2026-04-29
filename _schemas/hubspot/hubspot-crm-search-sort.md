---
description: A sort criterion for ordering search results.
layout: schema
name: Sort
properties_list:
- description: The name of the CRM property to sort by.
  name: propertyName
  type: string
- description: The sort direction.
  name: direction
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-search-sort-schema.json
slug: hubspot-crm-search-sort
source_filename: hubspot-crm-search-sort-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A sort criterion for ordering search results.\",\n  \"properties\": {\n    \"propertyName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the CRM property to sort by.\",\n      \"example\": \"Example Record\"\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"description\": \"The sort direction.\",\n      \"example\": \"ASCENDING\",\n      \"enum\": [\n        \"ASCENDING\",\n        \"DESCENDING\"\n      ]\n    }\n  },\n  \"required\": [\n    \"propertyName\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Sort\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-search-sort-schema.json
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
title: Sort
---
