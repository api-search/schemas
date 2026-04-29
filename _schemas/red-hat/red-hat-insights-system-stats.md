---
description: Aggregate statistics about registered systems.
layout: schema
name: SystemStats
properties_list:
- description: The total number of registered systems.
  name: total
  type: integer
- description: The number of stale systems.
  name: stale
  type: integer
- description: Systems with at least one active recommendation.
  name: with_hits
  type: integer
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-insights-system-stats-schema.json
slug: red-hat-insights-system-stats
source_filename: red-hat-insights-system-stats-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SystemStats\",\n  \"type\": \"object\",\n  \"description\": \"Aggregate statistics about registered systems.\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of registered systems.\"\n    },\n    \"stale\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of stale systems.\"\n    },\n    \"with_hits\": {\n      \"type\": \"integer\",\n      \"description\": \"Systems with at least one active recommendation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-insights-system-stats-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: SystemStats
---
