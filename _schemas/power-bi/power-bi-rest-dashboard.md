---
description: A Power BI dashboard
layout: schema
name: Dashboard
properties_list:
- description: The unique identifier of the dashboard
  name: id
  type: string
- description: The display name of the dashboard
  name: displayName
  type: string
- description: Whether the dashboard is read-only
  name: isReadOnly
  type: boolean
- description: The web URL of the dashboard
  name: webUrl
  type: string
- description: The embed URL for embedding the dashboard
  name: embedUrl
  type: string
- description: The data classification label
  name: dataClassification
  type: string
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-rest-dashboard-schema.json
slug: power-bi-rest-dashboard
source_filename: power-bi-rest-dashboard-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Dashboard\",\n  \"type\": \"object\",\n  \"description\": \"A Power BI dashboard\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the dashboard\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the dashboard\"\n    },\n    \"isReadOnly\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the dashboard is read-only\"\n    },\n    \"webUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The web URL of the dashboard\"\n    },\n    \"embedUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The embed URL for embedding the dashboard\"\n    },\n    \"dataClassification\": {\n      \"type\": \"string\",\n      \"description\": \"The data classification label\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-rest-dashboard-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: Dashboard
---
