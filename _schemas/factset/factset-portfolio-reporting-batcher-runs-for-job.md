---
description: Provides full details of when the job has been run
layout: schema
name: runsForJob
properties_list:
- description: The date and time the job was finished processing
  name: endTime
  type: string
- description: The ID of the run
  name: id
  type: string
- description: Indicates whether the job was triggered via the PRB API
  name: isApiTriggered
  type: boolean
- description: Number of seconds between startTime and endTime
  name: runDuration
  type: number
- description: The date and time the job started running after being submitted and potentially waiting in any queue
  name: startTime
  type: string
- description: The date and time the job was submitted
  name: submitTime
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-portfolio-reporting-batcher-runs-for-job-schema.json
slug: factset-portfolio-reporting-batcher-runs-for-job
source_filename: factset-portfolio-reporting-batcher-runs-for-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"runsForJob\",\n  \"type\": \"object\",\n  \"description\": \"Provides full details of when the job has been run\",\n  \"properties\": {\n    \"endTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the job was finished processing\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the run\"\n    },\n    \"isApiTriggered\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the job was triggered via the PRB API\"\n    },\n    \"runDuration\": {\n      \"type\": \"number\",\n      \"description\": \"Number of seconds between startTime and endTime\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the job started running after being submitted and potentially waiting in any queue\"\n    },\n    \"submitTime\": {\n      \"type\": \"string\",\n      \"\
  description\": \"The date and time the job was submitted\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-portfolio-reporting-batcher-runs-for-job-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: runsForJob
---
