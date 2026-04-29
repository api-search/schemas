---
description: Request body for creating a push dataset
layout: schema
name: CreateDatasetRequest
properties_list:
- description: The display name of the dataset
  name: name
  type: string
- description: The dataset mode
  name: defaultMode
  type: string
- description: The tables within the dataset
  name: tables
  type: array
- description: Relationships between tables
  name: relationships
  type: array
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-rest-create-dataset-request-schema.json
slug: power-bi-rest-create-dataset-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateDatasetRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a push dataset\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the dataset\"\n    },\n    \"defaultMode\": {\n      \"type\": \"string\",\n      \"description\": \"The dataset mode\"\n    },\n    \"tables\": {\n      \"type\": \"array\",\n      \"description\": \"The tables within the dataset\"\n    },\n    \"relationships\": {\n      \"type\": \"array\",\n      \"description\": \"Relationships between tables\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-rest-create-dataset-request-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: CreateDatasetRequest
---
