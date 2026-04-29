---
description: A group of filters (AND logic within group)
layout: schema
name: FilterGroup
properties_list:
- description: The filters in this group
  name: filters
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-engagement-calls-filter-group-schema.json
slug: hubspot-engagement-calls-filter-group
source_filename: hubspot-engagement-calls-filter-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A group of filters (AND logic within group)\",\n  \"properties\": {\n    \"filters\": {\n      \"type\": \"array\",\n      \"description\": \"The filters in this group\",\n      \"example\": [\n        {\n          \"propertyName\": \"hs_call_direction\",\n          \"operator\": \"EQ\",\n          \"value\": \"OUTBOUND\",\n          \"values\": [\n            {}\n          ],\n          \"highValue\": \"example-value\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A single search filter\",\n        \"properties\": {\n          \"propertyName\": {\n            \"type\": \"string\",\n            \"description\": \"The property to filter on\",\n            \"example\": \"hs_call_direction\"\n          },\n          \"operator\": {\n            \"type\": \"string\",\n            \"description\": \"The filter operator\",\n            \"example\": \"EQ\",\n            \"enum\"\
  : [\n              \"EQ\",\n              \"NEQ\",\n              \"LT\",\n              \"LTE\",\n              \"GT\",\n              \"GTE\",\n              \"BETWEEN\",\n              \"IN\",\n              \"NOT_IN\",\n              \"HAS_PROPERTY\",\n              \"NOT_HAS_PROPERTY\",\n              \"CONTAINS_TOKEN\",\n              \"NOT_CONTAINS_TOKEN\"\n            ]\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"description\": \"The value to filter by\",\n            \"example\": \"OUTBOUND\"\n          },\n          \"values\": {\n            \"type\": \"array\",\n            \"description\": \"Values for IN/NOT_IN operators\",\n            \"example\": [\n              \"example-value\"\n            ],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"highValue\": {\n            \"type\": \"string\",\n            \"description\": \"High value for BETWEEN operator\",\n          \
  \  \"example\": \"example-value\"\n          }\n        },\n        \"required\": [\n          \"propertyName\",\n          \"operator\"\n        ]\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FilterGroup\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-calls-filter-group-schema.json
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
