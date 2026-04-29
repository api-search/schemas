---
description: Contract for creating a new execution job
layout: schema
name: CreateJobContract
properties_list:
- description: Worker tag for routing
  name: workerTag
  type: string
- description: Credential to use for execution
  name: credentialId
  type: string
- description: Analytic app question values
  name: questions
  type: array
- description: Job priority
  name: priority
  type: string
provider_name: Alteryx
provider_slug: alteryx
schema_file: json-schema/alteryx-server-v3-create-job-contract-schema.json
slug: alteryx-server-v3-create-job-contract
source_filename: alteryx-server-v3-create-job-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateJobContract\",\n  \"type\": \"object\",\n  \"description\": \"Contract for creating a new execution job\",\n  \"properties\": {\n    \"workerTag\": {\n      \"type\": \"string\",\n      \"description\": \"Worker tag for routing\"\n    },\n    \"credentialId\": {\n      \"type\": \"string\",\n      \"description\": \"Credential to use for execution\"\n    },\n    \"questions\": {\n      \"type\": \"array\",\n      \"description\": \"Analytic app question values\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"description\": \"Job priority\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/json-schema/alteryx-server-v3-create-job-contract-schema.json
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
title: CreateJobContract
---
