---
description: Represents a metric value returned by the Azure Monitor Metrics API, containing time series data with aggregated values over specified intervals.
layout: schema
name: Azure Monitor Metric
properties_list:
- description: The metric ID, typically in the format of a fully qualified Azure resource ID with metric name.
  name: id
  type: string
- description: The resource type of the metric resource, typically Microsoft.Insights/metrics.
  name: type
  type: string
- description: The name of the metric.
  name: name
  type: object
- description: Detailed description of this metric.
  name: displayDescription
  type: string
- description: Error code encountered while querying this specific metric.
  name: errorCode
  type: string
- description: Error message encountered while querying this specific metric.
  name: errorMessage
  type: string
- description: The unit of the metric.
  name: unit
  type: object
- description: The time series returned when a data query is performed.
  name: timeseries
  type: array
provider_name: Azure Monitor
provider_slug: microsoft-azure-monitor
schema_file: json-schema/azure-monitor-metric-schema.json
slug: azure-monitor-metric
source_filename: azure-monitor-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.azure.com/monitor/metric.json\",\n  \"title\": \"Azure Monitor Metric\",\n  \"description\": \"Represents a metric value returned by the Azure Monitor Metrics API, containing time series data with aggregated values over specified intervals.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"type\", \"name\", \"unit\", \"timeseries\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The metric ID, typically in the format of a fully qualified Azure resource ID with metric name.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type of the metric resource, typically Microsoft.Insights/metrics.\"\n    },\n    \"name\": {\n      \"$ref\": \"#/$defs/LocalizableString\",\n      \"description\": \"The name of the metric.\"\n    },\n    \"displayDescription\": {\n      \"type\": \"string\",\n   \
  \   \"description\": \"Detailed description of this metric.\"\n    },\n    \"errorCode\": {\n      \"type\": \"string\",\n      \"description\": \"Error code encountered while querying this specific metric.\"\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Error message encountered while querying this specific metric.\"\n    },\n    \"unit\": {\n      \"$ref\": \"#/$defs/MetricUnit\",\n      \"description\": \"The unit of the metric.\"\n    },\n    \"timeseries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TimeSeriesElement\"\n      },\n      \"description\": \"The time series returned when a data query is performed.\"\n    }\n  },\n  \"$defs\": {\n    \"LocalizableString\": {\n      \"type\": \"object\",\n      \"required\": [\"value\"],\n      \"properties\": {\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The invariant value.\"\n        },\n        \"localizedValue\": {\n\
  \          \"type\": \"string\",\n          \"description\": \"The locale-specific display name.\"\n        }\n      }\n    },\n    \"MetricUnit\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Count\",\n        \"Bytes\",\n        \"Seconds\",\n        \"CountPerSecond\",\n        \"BytesPerSecond\",\n        \"Percent\",\n        \"MilliSeconds\",\n        \"ByteSeconds\",\n        \"Unspecified\",\n        \"Cores\",\n        \"MilliCores\",\n        \"NanoCores\",\n        \"BitsPerSecond\"\n      ],\n      \"description\": \"The unit of the metric.\"\n    },\n    \"TimeSeriesElement\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"metadatavalues\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/MetadataValue\"\n          },\n          \"description\": \"The metadata values returned if a metadata filter was specified.\"\n        },\n        \"data\": {\n          \"type\": \"array\",\n          \"items\"\
  : {\n            \"$ref\": \"#/$defs/MetricValue\"\n          },\n          \"description\": \"An array of data points representing the metric values.\"\n        }\n      }\n    },\n    \"MetadataValue\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"$ref\": \"#/$defs/LocalizableString\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The value of the metadata.\"\n        }\n      }\n    },\n    \"MetricValue\": {\n      \"type\": \"object\",\n      \"required\": [\"timeStamp\"],\n      \"properties\": {\n        \"timeStamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The timestamp for the metric value in ISO 8601 format.\"\n        },\n        \"average\": {\n          \"type\": \"number\",\n          \"description\": \"The average value in the time range.\"\n        },\n        \"minimum\": {\n          \"type\": \"number\",\n    \
  \      \"description\": \"The least value in the time range.\"\n        },\n        \"maximum\": {\n          \"type\": \"number\",\n          \"description\": \"The greatest value in the time range.\"\n        },\n        \"total\": {\n          \"type\": \"number\",\n          \"description\": \"The sum of all of the values in the time range.\"\n        },\n        \"count\": {\n          \"type\": \"number\",\n          \"description\": \"The number of samples in the time range.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-monitor/refs/heads/main/json-schema/azure-monitor-metric-schema.json
tags:
- Application Insights
- Cloud
- Logs
- Metrics
- Monitoring
- Observability
title: Azure Monitor Metric
---
