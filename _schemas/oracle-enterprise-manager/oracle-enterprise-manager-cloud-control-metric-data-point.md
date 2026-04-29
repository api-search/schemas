---
description: A single metric data point.
layout: schema
name: MetricDataPoint
properties_list:
- description: Name of the metric column.
  name: metricColumn
  type: string
- description: Numeric metric value.
  name: value
  type: number
- description: Key value identifying the metric row.
  name: key
  type: string
- description: Timestamp when the metric was collected.
  name: collectionTime
  type: string
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-cloud-control-metric-data-point-schema.json
slug: oracle-enterprise-manager-cloud-control-metric-data-point
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricDataPoint\",\n  \"type\": \"object\",\n  \"description\": \"A single metric data point.\",\n  \"properties\": {\n    \"metricColumn\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the metric column.\"\n    },\n    \"value\": {\n      \"type\": \"number\",\n      \"description\": \"Numeric metric value.\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Key value identifying the metric row.\"\n    },\n    \"collectionTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the metric was collected.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-cloud-control-metric-data-point-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: MetricDataPoint
---
