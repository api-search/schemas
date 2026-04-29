---
description: ApplicationSummary schema from oracle-cloud-functions-openapi.yaml
layout: schema
name: ApplicationSummary
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
  name: lifecycleState
  type: string
- description: ''
  name: timeCreated
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/functions-application-summary-schema.json
slug: functions-application-summary
source_filename: functions-application-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/functions-application-summary-schema.json\",\n  \"title\": \"ApplicationSummary\",\n  \"description\": \"ApplicationSummary schema from oracle-cloud-functions-openapi.yaml\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"example\": \"my-resource\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/functions-application-summary-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: ApplicationSummary
---
