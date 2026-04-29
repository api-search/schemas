---
description: JobList schema from Apache Pig
layout: schema
name: JobList
properties_list:
- description: ''
  name: jobs
  type: array
- description: ''
  name: total
  type: integer
provider_name: Apache Pig
provider_slug: apache-pig
schema_file: json-schema/apache-pig-job-list-schema.json
slug: apache-pig-job-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pig/refs/heads/main/json-schema/apache-pig-job-list-schema.json\",\n  \"title\": \"JobList\",\n  \"description\": \"JobList schema from Apache Pig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Job\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"example\": 5\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pig/refs/heads/main/json-schema/apache-pig-job-list-schema.json
tags:
- Big Data
- Data Analysis
- ETL
- Hadoop
- Scripting
- Apache
- Open Source
title: JobList
---
