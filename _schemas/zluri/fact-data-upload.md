---
description: Payload for uploading fact entity data within an active sync session. Fact data represents historical events appended to the timeline for analytics and compliance.
layout: schema
name: Zluri Fact Data Upload
properties_list:
- description: The type of fact entity being uploaded.
  name: entity
  type: string
- description: Page number for this batch of data.
  name: page
  type: integer
- description: Array of fact records. Maximum 1000 records per page.
  name: data
  type: array
provider_name: Zluri
provider_slug: zluri
schema_file: json-schema/fact-data-upload.json
slug: fact-data-upload
source_filename: fact-data-upload.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/zluri/refs/heads/main/json-schema/fact-data-upload.json\",\n  \"title\": \"Zluri Fact Data Upload\",\n  \"description\": \"Payload for uploading fact entity data within an active sync session. Fact data represents historical events appended to the timeline for analytics and compliance.\",\n  \"type\": \"object\",\n  \"required\": [\"entity\", \"page\", \"data\"],\n  \"properties\": {\n    \"entity\": {\n      \"type\": \"string\",\n      \"description\": \"The type of fact entity being uploaded.\",\n      \"enum\": [\"activities\", \"transactions\"]\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"description\": \"Page number for this batch of data.\",\n      \"minimum\": 1\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of fact records. Maximum 1000 records per page.\",\n      \"maxItems\": 1000,\n\
  \      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zluri/refs/heads/main/json-schema/fact-data-upload.json
tags:
- Access Management
- SaaS Management
title: Zluri Fact Data Upload
---
