---
description: UpdateAlarmDetails schema from oracle-cloud-monitoring-openapi.yaml
layout: schema
name: UpdateAlarmDetails
properties_list:
- description: ''
  name: displayName
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
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/monitoring-update-alarm-details-schema.json
slug: monitoring-update-alarm-details
source_filename: monitoring-update-alarm-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/monitoring-update-alarm-details-schema.json\",\n  \"title\": \"UpdateAlarmDetails\",\n  \"description\": \"UpdateAlarmDetails schema from oracle-cloud-monitoring-openapi.yaml\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\",\n      \"example\": \"my-resource\"\n    },\n    \"query\": {\n      \"type\": \"string\",\n      \"example\": \"CpuUtilization[1m].mean()\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    },\n    \"isEnabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/monitoring-update-alarm-details-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: UpdateAlarmDetails
---
