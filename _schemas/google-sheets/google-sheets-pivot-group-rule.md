---
description: An optional setting on a PivotGroup that defines buckets for the values in the source data column.
layout: schema
name: PivotGroupRule
properties_list:
- description: A ManualRule.
  name: manualRule
  type: object
- description: A HistogramRule.
  name: histogramRule
  type: object
- description: A DateTimeRule.
  name: dateTimeRule
  type: object
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-pivot-group-rule-schema.json
slug: google-sheets-pivot-group-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PivotGroupRule\",\n  \"type\": \"object\",\n  \"description\": \"An optional setting on a PivotGroup that defines buckets for the values in the source data column.\",\n  \"properties\": {\n    \"manualRule\": {\n      \"type\": \"object\",\n      \"description\": \"A ManualRule.\"\n    },\n    \"histogramRule\": {\n      \"type\": \"object\",\n      \"description\": \"A HistogramRule.\"\n    },\n    \"dateTimeRule\": {\n      \"type\": \"object\",\n      \"description\": \"A DateTimeRule.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-pivot-group-rule-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: PivotGroupRule
---
