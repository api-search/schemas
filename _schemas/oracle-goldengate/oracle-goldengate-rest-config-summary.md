---
description: ''
layout: schema
name: ConfigSummary
properties_list:
- description: ''
  name: serviceType
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: host
  type: string
- description: ''
  name: port
  type: integer
- description: ''
  name: deploymentName
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-config-summary-schema.json
slug: oracle-goldengate-rest-config-summary
source_filename: oracle-goldengate-rest-config-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConfigSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceType\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"host\": {\n      \"type\": \"string\"\n    },\n    \"port\": {\n      \"type\": \"integer\"\n    },\n    \"deploymentName\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-config-summary-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: ConfigSummary
---
