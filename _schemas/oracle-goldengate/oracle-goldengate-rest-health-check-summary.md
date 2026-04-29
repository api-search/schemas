---
description: ''
layout: schema
name: HealthCheckSummary
properties_list:
- description: ''
  name: healthy
  type: boolean
- description: ''
  name: status
  type: string
- description: ''
  name: timestamp
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-health-check-summary-schema.json
slug: oracle-goldengate-rest-health-check-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HealthCheckSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"healthy\": {\n      \"type\": \"boolean\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-health-check-summary-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: HealthCheckSummary
---
