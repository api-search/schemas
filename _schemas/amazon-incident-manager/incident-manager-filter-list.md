---
description: FilterList schema
layout: schema
name: FilterList
properties_list: []
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-filter-list-schema.json
slug: incident-manager-filter-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-filter-list-schema.json\",\n  \"title\": \"FilterList\",\n  \"description\": \"FilterList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"condition\",\n      \"key\"\n    ],\n    \"properties\": {\n      \"condition\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Condition\"\n          },\n          {\n            \"description\": \"The condition accepts before or after a specified time, equal to a string, or equal to an integer.\"\n          }\n        ]\n      },\n      \"key\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/FilterKeyString\"\n          },\n          {\n            \"description\": \"The key that you're filtering on.\"\n       \
  \   }\n        ]\n      }\n    },\n    \"description\": \"Filter the selection by using a condition.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-filter-list-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: FilterList
---
