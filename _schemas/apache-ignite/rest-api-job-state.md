---
description: Rest representation of org.apache.ignite.compute.JobState.
layout: schema
name: JobState
properties_list:
- description: Job ID.
  name: id
  type: string
- description: Job status.
  name: status
  type: object
- description: Job create time.
  name: createTime
  type: string
- description: Job start time.
  name: startTime
  type: string
- description: Job finish time.
  name: finishTime
  type: string
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-job-state-schema.json
slug: rest-api-job-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-job-state-schema.json\",\n  \"title\": \"JobState\",\n  \"description\": \"Rest representation of org.apache.ignite.compute.JobState.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Job ID.\",\n      \"format\": \"uuid\"\n    },\n    \"status\": {\n      \"description\": \"Job status.\",\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {}\n      ]\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"Job create time.\",\n      \"format\": \"date-time\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"description\": \"Job start time.\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"finishTime\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Job finish time.\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    }\n  },\n  \"required\": [\n    \"createTime\",\n    \"id\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-job-state-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: JobState
---
