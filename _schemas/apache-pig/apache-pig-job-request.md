---
description: JobRequest schema from Apache Pig
layout: schema
name: JobRequest
properties_list:
- description: Pig Latin script content
  name: script
  type: string
- description: Job name
  name: name
  type: string
- description: ''
  name: executionEngine
  type: string
- description: Script parameters as key-value pairs
  name: parameters
  type: object
provider_name: Apache Pig
provider_slug: apache-pig
schema_file: json-schema/apache-pig-job-request-schema.json
slug: apache-pig-job-request
source_filename: apache-pig-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pig/refs/heads/main/json-schema/apache-pig-job-request-schema.json\",\n  \"title\": \"JobRequest\",\n  \"description\": \"JobRequest schema from Apache Pig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"script\": {\n      \"type\": \"string\",\n      \"description\": \"Pig Latin script content\",\n      \"example\": \"A = LOAD 'data.csv' USING PigStorage(',');\\nB = FILTER A BY $0 > 100;\\nSTORE B INTO 'output';\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Job name\",\n      \"example\": \"sales-analysis\"\n    },\n    \"executionEngine\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"mapreduce\",\n        \"tez\",\n        \"local\"\n      ],\n      \"default\": \"tez\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\"\
  : \"string\"\n      },\n      \"description\": \"Script parameters as key-value pairs\"\n    }\n  },\n  \"required\": [\n    \"script\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pig/refs/heads/main/json-schema/apache-pig-job-request-schema.json
tags:
- Big Data
- Data Analysis
- ETL
- Hadoop
- Scripting
- Apache
- Open Source
title: JobRequest
---
