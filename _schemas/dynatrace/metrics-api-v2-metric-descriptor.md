---
description: Describes a single metric including its metadata, supported aggregations, entity dimensions, and default aggregation settings.
layout: schema
name: MetricDescriptor
properties_list:
- description: The fully qualified key of the metric, potentially including applied transformations. For example, builtin:host.cpu.usage:avg.
  name: metricId
  type: string
- description: The human-readable display name of the metric.
  name: displayName
  type: string
- description: A detailed description of what the metric measures.
  name: description
  type: string
- description: The unit of the metric values. For example, Percent, Byte, MilliSecond.
  name: unit
  type: string
- description: Whether ingesting this metric consumes Davis Data Units (DDUs).
  name: dduBillable
  type: boolean
- description: The Unix timestamp in milliseconds when the metric was created.
  name: created
  type: integer
- description: The Unix timestamp in milliseconds when the metric was last written.
  name: lastWritten
  type: integer
- description: The entity types that can be used to filter this metric, e.g., HOST, SERVICE, PROCESS_GROUP.
  name: entityType
  type: array
- description: The list of aggregation types supported for this metric. Valid values include min, max, sum, count, avg, median, and percentile.
  name: aggregationTypes
  type: array
- description: The list of dimension definitions for this metric. Each dimension provides a label for data splitting.
  name: dimensionDefinitions
  type: array
- description: The list of transformation expressions that can be applied to this metric using the metric selector.
  name: transformations
  type: array
- description: ''
  name: defaultAggregation
  type: object
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/metrics-api-v2-metric-descriptor-schema.json
slug: metrics-api-v2-metric-descriptor
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/metrics-api-v2-metric-descriptor-schema.json\",\n  \"title\": \"MetricDescriptor\",\n  \"description\": \"Describes a single metric including its metadata, supported aggregations, entity dimensions, and default aggregation settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metricId\": {\n      \"type\": \"string\",\n      \"description\": \"The fully qualified key of the metric, potentially including applied transformations. For example, builtin:host.cpu.usage:avg.\",\n      \"example\": \"abc123\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable display name of the metric.\",\n      \"example\": \"Production Service\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A detailed description of what the\
  \ metric measures.\",\n      \"example\": \"Example description.\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"The unit of the metric values. For example, Percent, Byte, MilliSecond.\",\n      \"example\": \"example-value\"\n    },\n    \"dduBillable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether ingesting this metric consumes Davis Data Units (DDUs).\",\n      \"example\": true\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The Unix timestamp in milliseconds when the metric was created.\",\n      \"example\": 500\n    },\n    \"lastWritten\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The Unix timestamp in milliseconds when the metric was last written.\",\n      \"example\": 500\n    },\n    \"entityType\": {\n      \"type\": \"array\",\n      \"description\": \"The entity types that can be used to filter this metric,\
  \ e.g., HOST, SERVICE, PROCESS_GROUP.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"STANDARD\"\n      ]\n    },\n    \"aggregationTypes\": {\n      \"type\": \"array\",\n      \"description\": \"The list of aggregation types supported for this metric. Valid values include min, max, sum, count, avg, median, and percentile.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"min\",\n          \"max\",\n          \"sum\",\n          \"count\",\n          \"avg\",\n          \"median\",\n          \"percentile\"\n        ]\n      },\n      \"example\": [\n        \"min\"\n      ]\n    },\n    \"dimensionDefinitions\": {\n      \"type\": \"array\",\n      \"description\": \"The list of dimension definitions for this metric. Each dimension provides a label for data splitting.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MetricDimensionDefinition\"\n      },\n      \"example\": [\n      \
  \  {\n          \"key\": \"example-value\",\n          \"name\": \"Production Service\",\n          \"type\": \"STANDARD\",\n          \"displayName\": \"Production Service\"\n        }\n      ]\n    },\n    \"transformations\": {\n      \"type\": \"array\",\n      \"description\": \"The list of transformation expressions that can be applied to this metric using the metric selector.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"example-value\"\n      ]\n    },\n    \"defaultAggregation\": {\n      \"$ref\": \"#/components/schemas/MetricDefaultAggregation\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/metrics-api-v2-metric-descriptor-schema.json
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
title: MetricDescriptor
---
