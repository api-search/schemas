---
description: A group of filters combined with AND logic
layout: schema
name: FilterGroup
properties_list:
- description: ''
  name: filters
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/commerce-payments-api-filter-group-schema.json
slug: commerce-payments-api-filter-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-filter-group-schema.json\",\n  \"title\": \"FilterGroup\",\n  \"description\": \"A group of filters combined with AND logic\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A single filter criterion\",\n        \"required\": [\n          \"propertyName\",\n          \"operator\"\n        ],\n        \"properties\": {\n          \"propertyName\": {\n            \"type\": \"string\",\n            \"description\": \"The property to filter on\",\n            \"example\": \"Example Record\"\n          },\n          \"operator\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"EQ\",\n              \"NEQ\",\n              \"LT\",\n        \
  \      \"LTE\",\n              \"GT\",\n              \"GTE\",\n              \"BETWEEN\",\n              \"IN\",\n              \"NOT_IN\",\n              \"HAS_PROPERTY\",\n              \"NOT_HAS_PROPERTY\",\n              \"CONTAINS_TOKEN\",\n              \"NOT_CONTAINS_TOKEN\"\n            ],\n            \"description\": \"The comparison operator\",\n            \"example\": \"EQ\"\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"description\": \"The value to compare against\",\n            \"example\": \"example-value\"\n          },\n          \"values\": {\n            \"type\": \"array\",\n            \"description\": \"Values for IN/NOT_IN operators\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"example\": [\n              \"example-value\"\n            ]\n          },\n          \"highValue\": {\n            \"type\": \"string\",\n            \"description\": \"Upper bound for BETWEEN operator\"\
  ,\n            \"example\": \"example-value\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"propertyName\": \"Example Record\",\n          \"operator\": \"EQ\",\n          \"value\": \"example-value\",\n          \"values\": [\n            {}\n          ],\n          \"highValue\": \"example-value\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"filters\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-filter-group-schema.json
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
title: FilterGroup
---
