---
description: A page within a Power BI report
layout: schema
name: Page
properties_list:
- description: The internal name of the page
  name: name
  type: string
- description: The display name shown in the report
  name: displayName
  type: string
- description: The order of the page within the report
  name: order
  type: integer
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-rest-page-schema.json
slug: power-bi-rest-page
source_filename: power-bi-rest-page-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Page\",\n  \"type\": \"object\",\n  \"description\": \"A page within a Power BI report\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The internal name of the page\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name shown in the report\"\n    },\n    \"order\": {\n      \"type\": \"integer\",\n      \"description\": \"The order of the page within the report\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-rest-page-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: Page
---
