---
description: List of Samza jobs
layout: schema
name: JobList
properties_list:
- description: ''
  name: jobs
  type: array
provider_name: Apache Samza
provider_slug: apache-samza
schema_file: json-schema/apache-samza-job-list-schema.json
slug: apache-samza-job-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-samza/refs/heads/main/json-schema/apache-samza-job-list-schema.json\",\n  \"title\": \"JobList\",\n  \"description\": \"List of Samza jobs\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Job\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-samza/refs/heads/main/json-schema/apache-samza-job-list-schema.json
tags:
- Big Data
- Hadoop
- Kafka
- Stream Processing
- Streaming
- Apache
- Open Source
title: JobList
---
