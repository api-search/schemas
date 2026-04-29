---
description: Definition of a data repair job
layout: schema
name: RepairJobDefinition
properties_list:
- description: Map of variable names to repair actions. Keys are Analytics variable names (e.g. eVar1, prop5, activitymap) and values are action objects.
  name: variables
  type: object
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-data-repair-repair-job-definition-schema.json
slug: adobe-analytics-data-repair-repair-job-definition
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Definition of a data repair job\",\n  \"properties\": {\n    \"variables\": {\n      \"type\": \"object\",\n      \"description\": \"Map of variable names to repair actions. Keys are Analytics variable names (e.g. eVar1, prop5, activitymap) and values are action objects.\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"variables\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RepairJobDefinition\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-data-repair-repair-job-definition-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: RepairJobDefinition
---
