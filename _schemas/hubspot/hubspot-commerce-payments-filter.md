---
description: A single filter criterion
layout: schema
name: Filter
properties_list:
- description: The property to filter on
  name: propertyName
  type: string
- description: The comparison operator
  name: operator
  type: string
- description: The value to compare against
  name: value
  type: string
- description: Values for IN/NOT_IN operators
  name: values
  type: array
- description: Upper bound for BETWEEN operator
  name: highValue
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-commerce-payments-filter-schema.json
slug: hubspot-commerce-payments-filter
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A single filter criterion\",\n  \"properties\": {\n    \"propertyName\": {\n      \"type\": \"string\",\n      \"description\": \"The property to filter on\",\n      \"example\": \"Example Record\"\n    },\n    \"operator\": {\n      \"type\": \"string\",\n      \"description\": \"The comparison operator\",\n      \"example\": \"EQ\",\n      \"enum\": [\n        \"EQ\",\n        \"NEQ\",\n        \"LT\",\n        \"LTE\",\n        \"GT\",\n        \"GTE\",\n        \"BETWEEN\",\n        \"IN\",\n        \"NOT_IN\",\n        \"HAS_PROPERTY\",\n        \"NOT_HAS_PROPERTY\",\n        \"CONTAINS_TOKEN\",\n        \"NOT_CONTAINS_TOKEN\"\n      ]\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value to compare against\",\n      \"example\": \"example-value\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"description\": \"Values for IN/NOT_IN operators\",\n      \"example\": [\n\
  \        \"example-value\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"highValue\": {\n      \"type\": \"string\",\n      \"description\": \"Upper bound for BETWEEN operator\",\n      \"example\": \"example-value\"\n    }\n  },\n  \"required\": [\n    \"propertyName\",\n    \"operator\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Filter\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-commerce-payments-filter-schema.json
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
