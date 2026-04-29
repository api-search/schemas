---
description: Aggregate statistics about Advisor rules.
layout: schema
name: RuleStats
properties_list:
- description: The total number of active rules.
  name: total
  type: integer
- description: Rule counts by category.
  name: by_category
  type: object
- description: Rule counts by total risk severity.
  name: by_severity
  type: object
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-insights-rule-stats-schema.json
slug: red-hat-insights-rule-stats
source_filename: red-hat-insights-rule-stats-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RuleStats\",\n  \"type\": \"object\",\n  \"description\": \"Aggregate statistics about Advisor rules.\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of active rules.\"\n    },\n    \"by_category\": {\n      \"type\": \"object\",\n      \"description\": \"Rule counts by category.\"\n    },\n    \"by_severity\": {\n      \"type\": \"object\",\n      \"description\": \"Rule counts by total risk severity.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-insights-rule-stats-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: RuleStats
---
