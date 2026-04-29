---
description: Optional filter to limit which rows are affected by the repair
layout: schema
name: RepairFilter
properties_list:
- description: The filter condition type
  name: condition
  type: string
- description: The value to match against for filtering
  name: matchValue
  type: string
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-data-repair-repair-filter-schema.json
slug: adobe-analytics-data-repair-repair-filter
source_filename: adobe-analytics-data-repair-repair-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Optional filter to limit which rows are affected by the repair\",\n  \"properties\": {\n    \"condition\": {\n      \"type\": \"string\",\n      \"description\": \"The filter condition type\",\n      \"example\": \"contains\",\n      \"enum\": [\n        \"contains\",\n        \"streq\",\n        \"startswith\"\n      ]\n    },\n    \"matchValue\": {\n      \"type\": \"string\",\n      \"description\": \"The value to match against for filtering\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RepairFilter\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-data-repair-repair-filter-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: RepairFilter
---
