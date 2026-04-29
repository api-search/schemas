---
description: A monitoring alarm.
layout: schema
name: Alarm
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: compartmentId
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: metricCompartmentId
  type: string
- description: ''
  name: namespace
  type: string
- description: ''
  name: query
  type: string
- description: ''
  name: severity
  type: string
- description: ''
  name: isEnabled
  type: boolean
- description: ''
  name: lifecycleState
  type: string
- description: ''
  name: destinations
  type: array
- description: ''
  name: timeCreated
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/monitoring-alarm-schema.json
slug: monitoring-alarm
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/monitoring-alarm-schema.json\",\n  \"title\": \"Alarm\",\n  \"description\": \"A monitoring alarm.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.alarm.oc1.iad.abcdefg123456\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"example\": \"High CPU Alarm\"\n    },\n    \"metricCompartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"example\": \"oci_computeagent\"\n    },\n    \"query\": {\n      \"type\": \"string\",\n      \"example\": \"CpuUtilization[1m].mean() > 90\"\n\
  \    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": \"['CRITICAL', 'ERROR', 'WARNING', 'INFO']\",\n      \"example\": \"CRITICAL\"\n    },\n    \"isEnabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"enum\": \"['ACTIVE', 'DELETING', 'DELETED']\",\n      \"example\": \"ACTIVE\"\n    },\n    \"destinations\": {\n      \"type\": \"array\",\n      \"example\": \"['example-value']\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/monitoring-alarm-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: Alarm
---
