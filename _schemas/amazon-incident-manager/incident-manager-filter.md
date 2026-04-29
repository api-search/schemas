---
description: Filter the selection by using a condition.
layout: schema
name: Filter
properties_list:
- description: ''
  name: condition
  type: object
- description: ''
  name: key
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-filter-schema.json
slug: incident-manager-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-filter-schema.json\",\n  \"title\": \"Filter\",\n  \"description\": \"Filter the selection by using a condition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"condition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Condition\"\n        },\n        {\n          \"description\": \"The condition accepts before or after a specified time, equal to a string, or equal to an integer.\"\n        }\n      ]\n    },\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterKeyString\"\n        },\n        {\n          \"description\": \"The key that you're filtering on.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"condition\",\n    \"key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-filter-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: Filter
---
