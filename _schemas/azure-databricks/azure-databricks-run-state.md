---
description: ''
layout: schema
name: RunState
properties_list:
- description: Life cycle state of the run
  name: life_cycle_state
  type: string
- description: Result state of the run (available after completion)
  name: result_state
  type: string
- description: Descriptive message for the current state
  name: state_message
  type: string
- description: Whether the run was cancelled by a user or timed out
  name: user_cancelled_or_timedout
  type: boolean
provider_name: Azure Databricks
provider_slug: azure-databricks
schema_file: json-schema/azure-databricks-run-state-schema.json
slug: azure-databricks-run-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RunState\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"life_cycle_state\": {\n      \"type\": \"string\",\n      \"description\": \"Life cycle state of the run\"\n    },\n    \"result_state\": {\n      \"type\": \"string\",\n      \"description\": \"Result state of the run (available after completion)\"\n    },\n    \"state_message\": {\n      \"type\": \"string\",\n      \"description\": \"Descriptive message for the current state\"\n    },\n    \"user_cancelled_or_timedout\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the run was cancelled by a user or timed out\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/json-schema/azure-databricks-run-state-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
title: RunState
---
