---
description: FilterGroup schema from HubSpot Engagement Tasks API
layout: schema
name: FilterGroup
properties_list:
- description: ''
  name: filters
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/engagement-tasks-api-filter-group-schema.json
slug: engagement-tasks-api-filter-group
source_filename: engagement-tasks-api-filter-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-tasks-api-filter-group-schema.json\",\n  \"title\": \"FilterGroup\",\n  \"description\": \"FilterGroup schema from HubSpot Engagement Tasks API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"propertyName\": {\n            \"type\": \"string\",\n            \"example\": \"Example Record\"\n          },\n          \"operator\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"EQ\",\n              \"NEQ\",\n              \"LT\",\n              \"LTE\",\n              \"GT\",\n              \"GTE\",\n              \"BETWEEN\",\n              \"IN\",\n              \"NOT_IN\",\n              \"HAS_PROPERTY\",\n              \"NOT_HAS_PROPERTY\"\
  ,\n              \"CONTAINS_TOKEN\",\n              \"NOT_CONTAINS_TOKEN\"\n            ],\n            \"example\": \"EQ\"\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"example\": \"example-value\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"propertyName\": \"Example Record\",\n          \"operator\": \"EQ\",\n          \"value\": \"example-value\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-tasks-api-filter-group-schema.json
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
