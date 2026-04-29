---
description: A pipeline component defining an activity, resource, schedule, or precondition.
layout: schema
name: Pipeline Object
properties_list:
- description: The identifier of the pipeline object
  name: id
  type: string
- description: The name
  name: name
  type: string
- description: ''
  name: fields
  type: array
provider_name: Amazon Data Pipeline
provider_slug: amazon-data-pipeline
schema_file: json-schema/pipeline-object-schema.json
slug: pipeline-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-pipeline/json-schema/pipeline-object-schema.json\",\n  \"title\": \"Pipeline Object\",\n  \"description\": \"A pipeline component defining an activity, resource, schedule, or precondition.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"fields\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the pipeline object\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name\"\n    },\n    \"fields\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/json-schema/pipeline-object-schema.json
tags:
- AWS
- Data Processing
- ETL
- Workflows
- Data Pipeline
- Automation
title: Pipeline Object
---
