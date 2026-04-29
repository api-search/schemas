---
description: Configuration for creating a new crawl job.
layout: schema
name: JobConfig
properties_list:
- description: The crawl identifier.
  name: crawlId
  type: string
- description: The type of Nutch crawl job.
  name: type
  type: string
- description: The configuration ID to use for this job. Defaults to "default" if not specified.
  name: confId
  type: string
- description: Fully qualified class name when type is CLASS.
  name: jobClassName
  type: string
- description: Additional arguments for the job.
  name: args
  type: object
provider_name: Apache Nutch
provider_slug: apache-nutch
schema_file: json-schema/apache-nutch-job-config-schema.json
slug: apache-nutch-job-config
source_filename: apache-nutch-job-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-job-config-schema.json\",\n  \"title\": \"JobConfig\",\n  \"description\": \"Configuration for creating a new crawl job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"crawlId\": {\n      \"type\": \"string\",\n      \"description\": \"The crawl identifier.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of Nutch crawl job.\",\n      \"enum\": [\n        \"INJECT\",\n        \"GENERATE\",\n        \"FETCH\",\n        \"PARSE\",\n        \"UPDATEDB\",\n        \"INDEX\",\n        \"READDB\",\n        \"CLASS\",\n        \"INVERTLINKS\",\n        \"DEDUP\"\n      ]\n    },\n    \"confId\": {\n      \"type\": \"string\",\n      \"description\": \"The configuration ID to use for this job. Defaults to \\\"default\\\" if not specified.\"\n    },\n\
  \    \"jobClassName\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified class name when type is CLASS.\"\n    },\n    \"args\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Additional arguments for the job.\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ],\n  \"example\": {\n    \"crawlId\": \"crawl-01\",\n    \"type\": \"INJECT\",\n    \"confId\": \"default\",\n    \"args\": {\n      \"seedDir\": \"seedFiles/seed-1700000000000\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-job-config-schema.json
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
title: JobConfig
---
