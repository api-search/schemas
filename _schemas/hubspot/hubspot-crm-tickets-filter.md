---
description: A single filter condition.
layout: schema
name: Filter
properties_list:
- description: ''
  name: propertyName
  type: string
- description: ''
  name: operator
  type: string
- description: ''
  name: value
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-tickets-filter-schema.json
slug: hubspot-crm-tickets-filter
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A single filter condition.\",\n  \"properties\": {\n    \"propertyName\": {\n      \"type\": \"string\",\n      \"example\": \"Example Record\"\n    },\n    \"operator\": {\n      \"type\": \"string\",\n      \"example\": \"EQ\",\n      \"enum\": [\n        \"EQ\",\n        \"NEQ\",\n        \"LT\",\n        \"LTE\",\n        \"GT\",\n        \"GTE\",\n        \"BETWEEN\",\n        \"IN\",\n        \"NOT_IN\",\n        \"HAS_PROPERTY\",\n        \"NOT_HAS_PROPERTY\",\n        \"CONTAINS_TOKEN\",\n        \"NOT_CONTAINS_TOKEN\"\n      ]\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Filter\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-tickets-filter-schema.json
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
title: Filter
---
