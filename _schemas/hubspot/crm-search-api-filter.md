---
description: A single filter condition for a CRM object property.
layout: schema
name: Filter
properties_list:
- description: The name of the CRM property to filter on.
  name: propertyName
  type: string
- description: The comparison operator for the filter.
  name: operator
  type: string
- description: The value to compare against. Not required for HAS_PROPERTY and NOT_HAS_PROPERTY operators.
  name: value
  type: string
- description: The upper bound value for BETWEEN operator comparisons.
  name: highValue
  type: string
- description: An array of values for IN and NOT_IN operator comparisons.
  name: values
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-search-api-filter-schema.json
slug: crm-search-api-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-search-api-filter-schema.json\",\n  \"title\": \"Filter\",\n  \"description\": \"A single filter condition for a CRM object property.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"propertyName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the CRM property to filter on.\",\n      \"example\": \"Example Record\"\n    },\n    \"operator\": {\n      \"type\": \"string\",\n      \"description\": \"The comparison operator for the filter.\",\n      \"enum\": [\n        \"EQ\",\n        \"NEQ\",\n        \"LT\",\n        \"LTE\",\n        \"GT\",\n        \"GTE\",\n        \"BETWEEN\",\n        \"IN\",\n        \"NOT_IN\",\n        \"HAS_PROPERTY\",\n        \"NOT_HAS_PROPERTY\",\n        \"CONTAINS_TOKEN\",\n        \"NOT_CONTAINS_TOKEN\"\n      ],\n      \"example\": \"EQ\"\n\
  \    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value to compare against. Not required for HAS_PROPERTY and NOT_HAS_PROPERTY operators.\",\n      \"example\": \"example-value\"\n    },\n    \"highValue\": {\n      \"type\": \"string\",\n      \"description\": \"The upper bound value for BETWEEN operator comparisons.\",\n      \"example\": \"example-value\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"An array of values for IN and NOT_IN operator comparisons.\",\n      \"example\": [\n        \"example-value\"\n      ]\n    }\n  },\n  \"required\": [\n    \"propertyName\",\n    \"operator\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-search-api-filter-schema.json
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
