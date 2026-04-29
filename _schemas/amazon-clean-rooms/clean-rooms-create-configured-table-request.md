---
description: Request body for creating a configured table.
layout: schema
name: CreateConfiguredTableRequest
properties_list:
- description: The name of the configured table.
  name: name
  type: string
- description: A description for the configured table.
  name: description
  type: string
- description: A reference to the AWS Glue table being configured.
  name: tableReference
  type: object
- description: The columns of the underlying AWS Glue table that can be used by collaborators.
  name: allowedColumns
  type: array
- description: The analysis method for the configured table.
  name: analysisMethod
  type: string
provider_name: Amazon Clean Rooms
provider_slug: amazon-clean-rooms
schema_file: json-schema/clean-rooms-create-configured-table-request-schema.json
slug: clean-rooms-create-configured-table-request
source_filename: clean-rooms-create-configured-table-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-create-configured-table-request-schema.json\",\n  \"title\": \"CreateConfiguredTableRequest\",\n  \"description\": \"Request body for creating a configured table.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the configured table.\",\n      \"example\": \"Customer Segments Table\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description for the configured table.\"\n    },\n    \"tableReference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to the AWS Glue table being configured.\"\n    },\n    \"allowedColumns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The columns\
  \ of the underlying AWS Glue table that can be used by collaborators.\"\n    },\n    \"analysisMethod\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"DIRECT_QUERY\"\n      ],\n      \"description\": \"The analysis method for the configured table.\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"tableReference\",\n    \"allowedColumns\",\n    \"analysisMethod\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-create-configured-table-request-schema.json
tags:
- AWS
- Clean Rooms
- Data Collaboration
- Privacy
- Analytics
- Marketing
title: CreateConfiguredTableRequest
---
