---
description: An analytic app question (input parameter)
layout: schema
name: WorkflowQuestion
properties_list:
- description: Name of the question
  name: name
  type: string
- description: Type of the question input
  name: questionType
  type: string
- description: Description of the question
  name: description
  type: string
- description: Default value
  name: value
  type: string
- description: Whether multiple selections are allowed
  name: multiple
  type: boolean
- description: Available options for the question
  name: items
  type: array
provider_name: Alteryx
provider_slug: alteryx
schema_file: json-schema/alteryx-server-v3-workflow-question-schema.json
slug: alteryx-server-v3-workflow-question
source_filename: alteryx-server-v3-workflow-question-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkflowQuestion\",\n  \"type\": \"object\",\n  \"description\": \"An analytic app question (input parameter)\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the question\"\n    },\n    \"questionType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the question input\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the question\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Default value\"\n    },\n    \"multiple\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether multiple selections are allowed\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"Available options for the question\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/json-schema/alteryx-server-v3-workflow-question-schema.json
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
title: WorkflowQuestion
---
