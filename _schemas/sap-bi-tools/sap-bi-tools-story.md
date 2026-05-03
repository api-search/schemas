---
description: Represents an analytic story in SAP Analytics Cloud. Stories are the primary visualization artifact containing charts, tables, and components for data analysis.
layout: schema
name: SAP Analytics Cloud Story
properties_list:
- description: The unique identifier of the story
  name: id
  type: string
- description: The display name of the story
  name: name
  type: string
- description: A text description of the story
  name: description
  type: string
- description: The timestamp when the story was created
  name: createdTime
  type: string
- description: The timestamp when the story was last modified
  name: modifiedTime
  type: string
- description: The user ID of the story creator
  name: createdBy
  type: string
- description: The user ID of the last modifier
  name: modifiedBy
  type: string
- description: The type of resource (always STORY)
  name: resourceType
  type: string
- description: List of models used in the story
  name: models
  type: array
provider_name: SAP BI Tools
provider_slug: sap-bi-tools
schema_file: json-schema/sap-bi-tools-story-schema.json
slug: sap-bi-tools-story
source_filename: sap-bi-tools-story-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/sap-bi-tools/json-schema/sap-bi-tools-story-schema.json\",\n  \"title\": \"SAP Analytics Cloud Story\",\n  \"description\": \"Represents an analytic story in SAP Analytics Cloud. Stories are the primary visualization artifact containing charts, tables, and components for data analysis.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the story\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the story\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A text description of the story\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the story was created\"\n    },\n    \"modifiedTime\": {\n\
  \      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the story was last modified\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"The user ID of the story creator\"\n    },\n    \"modifiedBy\": {\n      \"type\": \"string\",\n      \"description\": \"The user ID of the last modifier\"\n    },\n    \"resourceType\": {\n      \"type\": \"string\",\n      \"const\": \"STORY\",\n      \"description\": \"The type of resource (always STORY)\"\n    },\n    \"models\": {\n      \"type\": \"array\",\n      \"description\": \"List of models used in the story\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier of the model\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The display name of the model\"\n        \
  \  },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"A text description of the model\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/json-schema/sap-bi-tools-story-schema.json
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Reporting
- SAP
title: SAP Analytics Cloud Story
---
