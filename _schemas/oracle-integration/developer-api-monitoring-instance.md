---
description: MonitoringInstance schema from Oracle Integration Developer API.
layout: schema
name: MonitoringInstance
properties_list:
- description: Instance identifier.
  name: id
  type: string
- description: Parent integration identifier.
  name: integrationId
  type: string
- description: Instance status.
  name: status
  type: string
- description: Instance start time.
  name: startTime
  type: string
- description: Instance end time.
  name: endTime
  type: string
- description: Business identifier for the instance.
  name: businessIdentifier
  type: string
provider_name: Oracle Integration
provider_slug: oracle-integration
schema_file: json-schema/developer-api-monitoring-instance-schema.json
slug: developer-api-monitoring-instance
source_filename: developer-api-monitoring-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-integration/refs/heads/main/json-schema/developer-api-monitoring-instance-schema.json\",\n  \"title\": \"MonitoringInstance\",\n  \"description\": \"MonitoringInstance schema from Oracle Integration Developer API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\"type\": \"string\", \"description\": \"Instance identifier.\"},\n    \"integrationId\": {\"type\": \"string\", \"description\": \"Parent integration identifier.\"},\n    \"status\": {\"type\": \"string\", \"description\": \"Instance status.\", \"enum\": [\"COMPLETED\", \"FAILED\", \"ABORTED\", \"IN_PROGRESS\"]},\n    \"startTime\": {\"type\": \"string\", \"format\": \"date-time\", \"description\": \"Instance start time.\"},\n    \"endTime\": {\"type\": \"string\", \"format\": \"date-time\", \"description\": \"Instance end time.\"},\n    \"businessIdentifier\": {\"\
  type\": \"string\", \"description\": \"Business identifier for the instance.\"}\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-integration/refs/heads/main/json-schema/developer-api-monitoring-instance-schema.json
tags:
- API Management
- Automation
- B2B Integration
- Cloud Integration
- Enterprise Integration
- Integration
- iPaaS
- Process Automation
title: MonitoringInstance
---
