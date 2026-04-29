---
description: Information about a crawl job.
layout: schema
name: JobInfo
properties_list:
- description: The unique job identifier.
  name: id
  type: string
- description: The type of Nutch crawl job.
  name: type
  type: string
- description: The configuration ID used for this job.
  name: confId
  type: string
- description: Arguments passed to the job.
  name: args
  type: object
- description: Result data returned after job completion.
  name: result
  type: object
- description: The current state of a job.
  name: state
  type: string
- description: A human-readable status or error message.
  name: msg
  type: string
- description: The crawl identifier associated with this job.
  name: crawlId
  type: string
provider_name: Apache Nutch
provider_slug: apache-nutch
schema_file: json-schema/apache-nutch-job-info-schema.json
slug: apache-nutch-job-info
source_filename: apache-nutch-job-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-job-info-schema.json\",\n  \"title\": \"JobInfo\",\n  \"description\": \"Information about a crawl job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique job identifier.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of Nutch crawl job.\",\n      \"enum\": [\n        \"INJECT\",\n        \"GENERATE\",\n        \"FETCH\",\n        \"PARSE\",\n        \"UPDATEDB\",\n        \"INDEX\",\n        \"READDB\",\n        \"CLASS\",\n        \"INVERTLINKS\",\n        \"DEDUP\"\n      ]\n    },\n    \"confId\": {\n      \"type\": \"string\",\n      \"description\": \"The configuration ID used for this job.\"\n    },\n    \"args\": {\n      \"type\": \"object\",\n      \"additionalProperties\"\
  : true,\n      \"description\": \"Arguments passed to the job.\"\n    },\n    \"result\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Result data returned after job completion.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of a job.\",\n      \"enum\": [\n        \"IDLE\",\n        \"RUNNING\",\n        \"FINISHED\",\n        \"FAILED\",\n        \"KILLED\",\n        \"STOPPING\",\n        \"KILLING\",\n        \"ANY\"\n      ]\n    },\n    \"msg\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable status or error message.\"\n    },\n    \"crawlId\": {\n      \"type\": \"string\",\n      \"description\": \"The crawl identifier associated with this job.\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"state\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-job-info-schema.json
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
title: JobInfo
---
