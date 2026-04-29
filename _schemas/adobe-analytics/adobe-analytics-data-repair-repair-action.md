---
description: The action to take on a specific variable
layout: schema
name: RepairAction
properties_list:
- description: The repair action to perform
  name: action
  type: string
- description: The value to set the variable to (required when action is 'set')
  name: setValue
  type: string
- description: Optional filter to limit which rows are affected by the repair
  name: filter
  type: object
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-data-repair-repair-action-schema.json
slug: adobe-analytics-data-repair-repair-action
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"The action to take on a specific variable\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"The repair action to perform\",\n      \"example\": \"delete\",\n      \"enum\": [\n        \"delete\",\n        \"set\"\n      ]\n    },\n    \"setValue\": {\n      \"type\": \"string\",\n      \"description\": \"The value to set the variable to (required when action is 'set')\",\n      \"example\": \"example_value\"\n    },\n    \"filter\": {\n      \"type\": \"object\",\n      \"description\": \"Optional filter to limit which rows are affected by the repair\",\n      \"properties\": {\n        \"condition\": {\n          \"type\": \"string\",\n          \"description\": \"The filter condition type\",\n          \"example\": \"contains\",\n          \"enum\": [\n            \"contains\",\n            \"streq\",\n            \"startswith\"\n          ]\n        },\n        \"matchValue\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The value to match against for filtering\",\n          \"example\": \"example_value\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"action\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RepairAction\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-data-repair-repair-action-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: RepairAction
---
