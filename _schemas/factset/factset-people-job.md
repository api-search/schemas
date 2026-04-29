---
description: Basic information about a person's `Job`.
layout: schema
name: job
properties_list:
- description: City the job is located in.
  name: companyCity
  type: string
- description: FactSet Identifier for the company.
  name: companyId
  type: string
- description: Name of the company.
  name: companyName
  type: string
- description: Ending date for the Job.
  name: jobEndDate
  type: string
- description: Job function code.
  name: jobFunctionCode
  type: string
- description: Description of the job.
  name: jobFunctionName
  type: string
- description: Starting date for the Job.
  name: jobStartDate
  type: string
- description: Job Title
  name: jobTitle
  type: string
- description: FactSet Entity Identifier for the Person.
  name: personId
  type: string
- description: Original identifier used for the request.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-people-job-schema.json
slug: factset-people-job
source_filename: factset-people-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"job\",\n  \"type\": \"object\",\n  \"description\": \"Basic information about a person's `Job`.\",\n  \"properties\": {\n    \"companyCity\": {\n      \"type\": \"string\",\n      \"description\": \"City the job is located in.\"\n    },\n    \"companyId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Identifier for the company.\"\n    },\n    \"companyName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the company.\"\n    },\n    \"jobEndDate\": {\n      \"type\": \"string\",\n      \"description\": \"Ending date for the Job.\"\n    },\n    \"jobFunctionCode\": {\n      \"type\": \"string\",\n      \"description\": \"Job function code.\"\n    },\n    \"jobFunctionName\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the job.\"\n    },\n    \"jobStartDate\": {\n      \"type\": \"string\",\n      \"description\": \"Starting date\
  \ for the Job.\"\n    },\n    \"jobTitle\": {\n      \"type\": \"string\",\n      \"description\": \"Job Title\"\n    },\n    \"personId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Entity Identifier for the Person.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Original identifier used for the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-people-job-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: job
---
