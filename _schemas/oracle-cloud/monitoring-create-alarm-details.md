---
description: CreateAlarmDetails schema from oracle-cloud-monitoring-openapi.yaml
layout: schema
name: CreateAlarmDetails
properties_list:
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
  name: destinations
  type: array
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/monitoring-create-alarm-details-schema.json
slug: monitoring-create-alarm-details
source_filename: monitoring-create-alarm-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/monitoring-create-alarm-details-schema.json\",\n  \"title\": \"CreateAlarmDetails\",\n  \"description\": \"CreateAlarmDetails schema from oracle-cloud-monitoring-openapi.yaml\",\n  \"type\": \"object\",\n  \"required\": [\n    \"compartmentId\",\n    \"displayName\",\n    \"metricCompartmentId\",\n    \"namespace\",\n    \"query\",\n    \"severity\",\n    \"isEnabled\",\n    \"destinations\"\n  ],\n  \"properties\": {\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"example\": \"my-resource\"\n    },\n    \"metricCompartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"namespace\": {\n      \"type\": \"string\"\
  ,\n      \"example\": \"oci_computeagent\"\n    },\n    \"query\": {\n      \"type\": \"string\",\n      \"example\": \"CpuUtilization[1m].mean()\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": \"['CRITICAL', 'ERROR', 'WARNING', 'INFO']\",\n      \"example\": \"CRITICAL\"\n    },\n    \"isEnabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"destinations\": {\n      \"type\": \"array\",\n      \"example\": \"['example-value']\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/monitoring-create-alarm-details-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: CreateAlarmDetails
---
