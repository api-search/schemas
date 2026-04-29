---
description: A dataset refresh operation entry
layout: schema
name: Refresh
properties_list:
- description: The unique identifier of the refresh request
  name: requestId
  type: string
- description: The sequential identifier of the refresh
  name: id
  type: integer
- description: The type of refresh
  name: refreshType
  type: string
- description: The start time of the refresh
  name: startTime
  type: string
- description: The end time of the refresh
  name: endTime
  type: string
- description: The status of the refresh
  name: status
  type: string
- description: JSON-formatted error details if the refresh failed
  name: serviceExceptionJson
  type: string
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-rest-refresh-schema.json
slug: power-bi-rest-refresh
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Refresh\",\n  \"type\": \"object\",\n  \"description\": \"A dataset refresh operation entry\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the refresh request\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The sequential identifier of the refresh\"\n    },\n    \"refreshType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of refresh\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"description\": \"The start time of the refresh\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"description\": \"The end time of the refresh\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the refresh\"\n    },\n    \"serviceExceptionJson\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"JSON-formatted error details if the refresh failed\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-rest-refresh-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: Refresh
---
