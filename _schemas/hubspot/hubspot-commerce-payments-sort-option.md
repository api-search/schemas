---
description: A sort option for ordering results
layout: schema
name: SortOption
properties_list:
- description: The property to sort by
  name: propertyName
  type: string
- description: The sort direction
  name: direction
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-commerce-payments-sort-option-schema.json
slug: hubspot-commerce-payments-sort-option
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A sort option for ordering results\",\n  \"properties\": {\n    \"propertyName\": {\n      \"type\": \"string\",\n      \"description\": \"The property to sort by\",\n      \"example\": \"Example Record\"\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"description\": \"The sort direction\",\n      \"example\": \"ASCENDING\",\n      \"enum\": [\n        \"ASCENDING\",\n        \"DESCENDING\"\n      ]\n    }\n  },\n  \"required\": [\n    \"propertyName\",\n    \"direction\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SortOption\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-commerce-payments-sort-option-schema.json
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
