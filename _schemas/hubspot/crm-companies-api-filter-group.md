---
description: A group of filters combined with AND logic.
layout: schema
name: FilterGroup
properties_list:
- description: ''
  name: filters
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-companies-api-filter-group-schema.json
slug: crm-companies-api-filter-group
source_filename: crm-companies-api-filter-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-companies-api-filter-group-schema.json\",\n  \"title\": \"FilterGroup\",\n  \"description\": \"A group of filters combined with AND logic.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A single filter condition.\",\n        \"properties\": {\n          \"propertyName\": {\n            \"type\": \"string\",\n            \"example\": \"Example Record\"\n          },\n          \"operator\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"EQ\",\n              \"NEQ\",\n              \"LT\",\n              \"LTE\",\n              \"GT\",\n              \"GTE\",\n              \"BETWEEN\",\n              \"IN\",\n              \"NOT_IN\",\n            \
  \  \"HAS_PROPERTY\",\n              \"NOT_HAS_PROPERTY\",\n              \"CONTAINS_TOKEN\",\n              \"NOT_CONTAINS_TOKEN\"\n            ],\n            \"example\": \"EQ\"\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"example\": \"example-value\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"propertyName\": \"Example Record\",\n          \"operator\": \"EQ\",\n          \"value\": \"example-value\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-companies-api-filter-group-schema.json
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
