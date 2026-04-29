---
description: A Power BI report
layout: schema
name: Report
properties_list:
- description: The unique identifier of the report
  name: id
  type: string
- description: The display name of the report
  name: name
  type: string
- description: The ID of the dataset associated with this report
  name: datasetId
  type: string
- description: The web URL of the report
  name: webUrl
  type: string
- description: The embed URL for embedding the report in applications
  name: embedUrl
  type: string
- description: The type of the report
  name: reportType
  type: string
- description: The report description
  name: description
  type: string
- description: When the report was created
  name: createdDateTime
  type: string
- description: When the report was last modified
  name: modifiedDateTime
  type: string
- description: The user who last modified the report
  name: modifiedBy
  type: string
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-rest-report-schema.json
slug: power-bi-rest-report
source_filename: power-bi-rest-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Report\",\n  \"type\": \"object\",\n  \"description\": \"A Power BI report\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the report\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the report\"\n    },\n    \"datasetId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the dataset associated with this report\"\n    },\n    \"webUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The web URL of the report\"\n    },\n    \"embedUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The embed URL for embedding the report in applications\"\n    },\n    \"reportType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the report\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\":\
  \ \"The report description\"\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"When the report was created\"\n    },\n    \"modifiedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"When the report was last modified\"\n    },\n    \"modifiedBy\": {\n      \"type\": \"string\",\n      \"description\": \"The user who last modified the report\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-rest-report-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: Report
---
