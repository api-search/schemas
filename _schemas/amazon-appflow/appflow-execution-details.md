---
description: ExecutionDetails schema from Amazon AppFlow API
layout: schema
name: ExecutionDetails
properties_list:
- description: Describes the details of the most recent flow run.
  name: mostRecentExecutionMessage
  type: string
- description: Specifies the time of the most recent flow run.
  name: mostRecentExecutionTime
  type: integer
- description: Specifies the status of the most recent flow run.
  name: mostRecentExecutionStatus
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-execution-details-schema.json
slug: appflow-execution-details
source_filename: appflow-execution-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-execution-details-schema.json\",\n  \"title\": \"ExecutionDetails\",\n  \"description\": \"ExecutionDetails schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mostRecentExecutionMessage\": {\n      \"type\": \"string\",\n      \"example\": \"Successfully ran the flow\",\n      \"description\": \"Describes the details of the most recent flow run.\"\n    },\n    \"mostRecentExecutionTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1718153700000,\n      \"description\": \"Specifies the time of the most recent flow run.\"\n    },\n    \"mostRecentExecutionStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"InProgress\",\n        \"Successful\",\n        \"Error\",\n        \"CancelStarted\",\n        \"Canceled\"\
  \n      ],\n      \"example\": \"Successful\",\n      \"description\": \"Specifies the status of the most recent flow run.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-execution-details-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: ExecutionDetails
---
