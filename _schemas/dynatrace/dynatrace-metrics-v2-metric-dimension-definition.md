---
description: Defines a single dimension of a metric.
layout: schema
name: MetricDimensionDefinition
properties_list:
- description: The unique key identifying this dimension.
  name: key
  type: string
- description: The display name of the dimension.
  name: name
  type: string
- description: The type of the dimension. For example, ENTITY for entity dimensions or STRING for string dimensions.
  name: type
  type: string
- description: The human-readable display name of the dimension.
  name: displayName
  type: string
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/dynatrace-metrics-v2-metric-dimension-definition-schema.json
slug: dynatrace-metrics-v2-metric-dimension-definition
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Defines a single dimension of a metric.\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The unique key identifying this dimension.\",\n      \"example\": \"example-value\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the dimension.\",\n      \"example\": \"Production Service\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the dimension. For example, ENTITY for entity dimensions or STRING for string dimensions.\",\n      \"example\": \"STANDARD\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable display name of the dimension.\",\n      \"example\": \"Production Service\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricDimensionDefinition\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-metrics-v2-metric-dimension-definition-schema.json
tags:
- AI Operations
- Analytics
- APM
- Application Performance Monitoring
- Application Security
- Automation
- Cloud Monitoring
- Digital Experience Management
- Intelligence
- Observability
title: MetricDimensionDefinition
---
