---
description: Filter schema from HubSpot Engagement Emails API
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
schema_file: json-schema/engagement-emails-api-filter-schema.json
slug: engagement-emails-api-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-emails-api-filter-schema.json\",\n  \"title\": \"Filter\",\n  \"description\": \"Filter schema from HubSpot Engagement Emails API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"propertyName\": {\n      \"type\": \"string\",\n      \"example\": \"Example Record\"\n    },\n    \"operator\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"EQ\",\n        \"NEQ\",\n        \"LT\",\n        \"LTE\",\n        \"GT\",\n        \"GTE\",\n        \"BETWEEN\",\n        \"IN\",\n        \"NOT_IN\",\n        \"HAS_PROPERTY\",\n        \"NOT_HAS_PROPERTY\",\n        \"CONTAINS_TOKEN\",\n        \"NOT_CONTAINS_TOKEN\"\n      ],\n      \"example\": \"EQ\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-emails-api-filter-schema.json
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
