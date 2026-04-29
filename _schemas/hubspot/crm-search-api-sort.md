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
schema_file: json-schema/crm-search-api-sort-schema.json
slug: crm-search-api-sort
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-search-api-sort-schema.json\",\n  \"title\": \"Sort\",\n  \"description\": \"A sort criterion for ordering search results.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"propertyName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the CRM property to sort by.\",\n      \"example\": \"Example Record\"\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"description\": \"The sort direction.\",\n      \"enum\": [\n        \"ASCENDING\",\n        \"DESCENDING\"\n      ],\n      \"default\": \"ASCENDING\",\n      \"example\": \"ASCENDING\"\n    }\n  },\n  \"required\": [\n    \"propertyName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-search-api-sort-schema.json
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
