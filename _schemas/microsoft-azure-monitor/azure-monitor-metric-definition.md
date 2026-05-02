---
description: Represents a metric definition describing a metric that is available for an Azure resource, including its name, unit, available aggregation types, and time granularities.
layout: schema
name: Azure Monitor Metric Definition
properties_list:
- description: Flag to indicate whether the dimension is required.
  name: isDimensionRequired
  type: boolean
- description: The resource identifier of the resource that emitted the metric.
  name: resourceId
  type: string
- description: The namespace the metric belongs to.
  name: namespace
  type: string
- description: The name information for the metric.
  name: name
  type: object
- description: Detailed description of this metric.
  name: displayDescription
  type: string
- description: Custom category name for this metric.
  name: category
  type: string
- description: The class of the metric.
  name: metricClass
  type: string
- description: The unit of the metric.
  name: unit
  type: string
- description: The primary aggregation type value defining how to use the values for display.
  name: primaryAggregationType
  type: string
- description: The collection of what aggregation types are supported.
  name: supportedAggregationTypes
  type: array
- description: The collection of what aggregation intervals are available to be queried.
  name: metricAvailabilities
  type: array
- description: The resource identifier of the metric definition.
  name: id
  type: string
- description: The available dimensions for this metric.
  name: dimensions
  type: array
provider_name: Azure Monitor
provider_slug: microsoft-azure-monitor
schema_file: json-schema/azure-monitor-metric-definition-schema.json
slug: azure-monitor-metric-definition
source_filename: azure-monitor-metric-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.azure.com/monitor/metric-definition.json\",\n  \"title\": \"Azure Monitor Metric Definition\",\n  \"description\": \"Represents a metric definition describing a metric that is available for an Azure resource, including its name, unit, available aggregation types, and time granularities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"isDimensionRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag to indicate whether the dimension is required.\"\n    },\n    \"resourceId\": {\n      \"type\": \"string\",\n      \"description\": \"The resource identifier of the resource that emitted the metric.\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace the metric belongs to.\"\n    },\n    \"name\": {\n      \"$ref\": \"#/$defs/LocalizableString\",\n      \"description\": \"The name information for the metric.\"\
  \n    },\n    \"displayDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of this metric.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Custom category name for this metric.\"\n    },\n    \"metricClass\": {\n      \"type\": \"string\",\n      \"enum\": [\"Availability\", \"Transactions\", \"Errors\", \"Latency\", \"Saturation\"],\n      \"description\": \"The class of the metric.\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Count\", \"Bytes\", \"Seconds\", \"CountPerSecond\", \"BytesPerSecond\",\n        \"Percent\", \"MilliSeconds\", \"ByteSeconds\", \"Unspecified\",\n        \"Cores\", \"MilliCores\", \"NanoCores\", \"BitsPerSecond\"\n      ],\n      \"description\": \"The unit of the metric.\"\n    },\n    \"primaryAggregationType\": {\n      \"type\": \"string\",\n      \"enum\": [\"None\", \"Average\", \"Count\", \"Minimum\", \"Maximum\", \"Total\"],\n      \"\
  description\": \"The primary aggregation type value defining how to use the values for display.\"\n    },\n    \"supportedAggregationTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"None\", \"Average\", \"Count\", \"Minimum\", \"Maximum\", \"Total\"]\n      },\n      \"description\": \"The collection of what aggregation types are supported.\"\n    },\n    \"metricAvailabilities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/MetricAvailability\"\n      },\n      \"description\": \"The collection of what aggregation intervals are available to be queried.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The resource identifier of the metric definition.\"\n    },\n    \"dimensions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/LocalizableString\"\n      },\n      \"description\": \"The available dimensions for this metric.\"\n \
  \   }\n  },\n  \"$defs\": {\n    \"LocalizableString\": {\n      \"type\": \"object\",\n      \"required\": [\"value\"],\n      \"properties\": {\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The invariant value.\"\n        },\n        \"localizedValue\": {\n          \"type\": \"string\",\n          \"description\": \"The locale-specific display name.\"\n        }\n      }\n    },\n    \"MetricAvailability\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"timeGrain\": {\n          \"type\": \"string\",\n          \"description\": \"The time grain specifies the aggregation interval for the metric in ISO 8601 duration format.\"\n        },\n        \"retention\": {\n          \"type\": \"string\",\n          \"description\": \"The retention period for the metric at the specified time grain in ISO 8601 duration format.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-monitor/refs/heads/main/json-schema/azure-monitor-metric-definition-schema.json
tags:
- Application Insights
- Cloud
- Logs
- Metrics
- Monitoring
- Observability
title: Azure Monitor Metric Definition
---
