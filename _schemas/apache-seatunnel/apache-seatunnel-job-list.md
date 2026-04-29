---
description: List of SeaTunnel jobs
layout: schema
name: JobList
properties_list:
- description: ''
  name: jobs
  type: array
- description: ''
  name: total
  type: integer
provider_name: Apache SeaTunnel
provider_slug: apache-seatunnel
schema_file: json-schema/apache-seatunnel-job-list-schema.json
slug: apache-seatunnel-job-list
source_filename: apache-seatunnel-job-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-seatunnel/refs/heads/main/json-schema/apache-seatunnel-job-list-schema.json\",\n  \"title\": \"JobList\",\n  \"description\": \"List of SeaTunnel jobs\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/JobInfo\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-seatunnel/refs/heads/main/json-schema/apache-seatunnel-job-list-schema.json
tags:
- Data Integration
- ETL
- ELT
- Batch
- Streaming
- Apache
- Open Source
title: JobList
---
