---
description: Time series data for a single metric.
layout: schema
name: MetricTimeSeries
properties_list:
- description: Name of the target.
  name: targetName
  type: string
- description: Type of the target.
  name: targetType
  type: string
- description: Name of the metric group.
  name: metricGroupName
  type: string
- description: Name of the metric column.
  name: metricColumnName
  type: string
- description: Key value for the metric row.
  name: key
  type: string
- description: ''
  name: dataPoints
  type: array
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-cloud-control-metric-time-series-schema.json
slug: oracle-enterprise-manager-cloud-control-metric-time-series
source_filename: oracle-enterprise-manager-cloud-control-metric-time-series-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricTimeSeries\",\n  \"type\": \"object\",\n  \"description\": \"Time series data for a single metric.\",\n  \"properties\": {\n    \"targetName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the target.\"\n    },\n    \"targetType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the target.\"\n    },\n    \"metricGroupName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the metric group.\"\n    },\n    \"metricColumnName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the metric column.\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Key value for the metric row.\"\n    },\n    \"dataPoints\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-cloud-control-metric-time-series-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: MetricTimeSeries
---
