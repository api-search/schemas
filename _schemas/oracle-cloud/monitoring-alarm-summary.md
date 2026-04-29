---
description: AlarmSummary schema from oracle-cloud-monitoring-openapi.yaml
layout: schema
name: AlarmSummary
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: displayName
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
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/monitoring-alarm-summary-schema.json
slug: monitoring-alarm-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/monitoring-alarm-summary-schema.json\",\n  \"title\": \"AlarmSummary\",\n  \"description\": \"AlarmSummary schema from oracle-cloud-monitoring-openapi.yaml\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"example\": \"my-resource\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    },\n    \"isEnabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/monitoring-alarm-summary-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: AlarmSummary
---
