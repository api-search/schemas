---
description: A Power BI workspace (group)
layout: schema
name: Group
properties_list:
- description: The unique identifier of the workspace
  name: id
  type: string
- description: The display name of the workspace
  name: name
  type: string
- description: Whether the workspace is read-only
  name: isReadOnly
  type: boolean
- description: Whether the workspace is on a dedicated capacity
  name: isOnDedicatedCapacity
  type: boolean
- description: The capacity ID if on a dedicated capacity
  name: capacityId
  type: string
- description: The workspace type
  name: type
  type: string
- description: The workspace state
  name: state
  type: string
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-rest-group-schema.json
slug: power-bi-rest-group
source_filename: power-bi-rest-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Group\",\n  \"type\": \"object\",\n  \"description\": \"A Power BI workspace (group)\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the workspace\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the workspace\"\n    },\n    \"isReadOnly\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the workspace is read-only\"\n    },\n    \"isOnDedicatedCapacity\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the workspace is on a dedicated capacity\"\n    },\n    \"capacityId\": {\n      \"type\": \"string\",\n      \"description\": \"The capacity ID if on a dedicated capacity\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The workspace type\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"\
  description\": \"The workspace state\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-rest-group-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: Group
---
