---
description: A single filter condition.
layout: schema
name: Filter
properties_list:
- description: The name of the property to filter on.
  name: propertyName
  type: string
- description: The filter operator.
  name: operator
  type: string
- description: The value to compare against.
  name: value
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-contacts-api-filter-schema.json
slug: crm-contacts-api-filter
source_filename: crm-contacts-api-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-contacts-api-filter-schema.json\",\n  \"title\": \"Filter\",\n  \"description\": \"A single filter condition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"propertyName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the property to filter on.\",\n      \"example\": \"Example Record\"\n    },\n    \"operator\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"EQ\",\n        \"NEQ\",\n        \"LT\",\n        \"LTE\",\n        \"GT\",\n        \"GTE\",\n        \"BETWEEN\",\n        \"IN\",\n        \"NOT_IN\",\n        \"HAS_PROPERTY\",\n        \"NOT_HAS_PROPERTY\",\n        \"CONTAINS_TOKEN\",\n        \"NOT_CONTAINS_TOKEN\"\n      ],\n      \"description\": \"The filter operator.\",\n      \"example\": \"EQ\"\n    },\n    \"value\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The value to compare against.\",\n      \"example\": \"example-value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-contacts-api-filter-schema.json
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
