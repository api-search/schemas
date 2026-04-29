---
description: Contains pipeline metadata including name, description, fields, and tags.
layout: schema
name: Pipeline Description
properties_list:
- description: The unique identifier of the pipeline
  name: pipelineId
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: pipelineState
  type: string
provider_name: Amazon Data Pipeline
provider_slug: amazon-data-pipeline
schema_file: json-schema/pipeline-description-schema.json
slug: pipeline-description
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-pipeline/json-schema/pipeline-description-schema.json\",\n  \"title\": \"Pipeline Description\",\n  \"description\": \"Contains pipeline metadata including name, description, fields, and tags.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the pipeline\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"pipelineState\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SCHEDULED\",\n        \"RUNNING\",\n        \"SHUTTING_DOWN\",\n        \"FINISHED\",\n        \"FAILED\",\n        \"INACTIVE\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/json-schema/pipeline-description-schema.json
tags:
- AWS
- Data Processing
- ETL
- Workflows
- Data Pipeline
- Automation
title: Pipeline Description
---
