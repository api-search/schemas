---
description: Response after creating a pipeline.
layout: schema
name: Create Pipeline Output
properties_list:
- description: The unique identifier for the pipeline
  name: pipelineId
  type: string
provider_name: Amazon Data Pipeline
provider_slug: amazon-data-pipeline
schema_file: json-schema/create-pipeline-output-schema.json
slug: create-pipeline-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-pipeline/json-schema/create-pipeline-output-schema.json\",\n  \"title\": \"Create Pipeline Output\",\n  \"description\": \"Response after creating a pipeline.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the pipeline\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/json-schema/create-pipeline-output-schema.json
tags:
- AWS
- Data Processing
- ETL
- Workflows
- Data Pipeline
- Automation
title: Create Pipeline Output
---
