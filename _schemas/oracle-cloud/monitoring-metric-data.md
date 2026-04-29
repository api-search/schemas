---
description: Aggregated metric data points.
layout: schema
name: MetricData
properties_list:
- description: ''
  name: namespace
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: compartmentId
  type: string
- description: ''
  name: dimensions
  type: object
- description: ''
  name: aggregatedDatapoints
  type: array
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/monitoring-metric-data-schema.json
slug: monitoring-metric-data
source_filename: monitoring-metric-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/monitoring-metric-data-schema.json\",\n  \"title\": \"MetricData\",\n  \"description\": \"Aggregated metric data points.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"type\": \"string\",\n      \"example\": \"oci_computeagent\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"CpuUtilization\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"dimensions\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key1\": \"value1\"\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"aggregatedDatapoints\": {\n      \"type\": \"array\",\n      \"example\": \"[{'timestamp': '2026-04-18T10:30:00Z', 'value': 42.5}]\"\
  ,\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/monitoring-metric-data-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: MetricData
---
