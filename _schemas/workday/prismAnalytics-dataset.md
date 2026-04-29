---
description: ''
layout: schema
name: Dataset
properties_list:
- description: The Workday ID of the dataset.
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: The name of the dataset.
  name: name
  type: string
- description: The display name of the dataset.
  name: displayName
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: tags
  type: array
- description: ''
  name: fields
  type: array
- description: The number of rows in the dataset.
  name: rowCount
  type: integer
- description: ''
  name: createdOn
  type: string
- description: ''
  name: updatedOn
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/prismAnalytics-dataset-schema.json
slug: prismAnalytics-dataset
source_filename: prismAnalytics-dataset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Dataset\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Workday ID of the dataset.\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the dataset.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the dataset.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"fields\": {\n      \"type\": \"array\"\n    },\n    \"rowCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of rows in the dataset.\"\n    },\n    \"createdOn\": {\n      \"type\": \"string\"\n    },\n    \"updatedOn\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/prismAnalytics-dataset-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: Dataset
---
