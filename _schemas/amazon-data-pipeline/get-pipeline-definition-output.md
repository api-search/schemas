---
description: Response containing the pipeline definition.
layout: schema
name: Get Pipeline Definition Output
properties_list:
- description: ''
  name: pipelineObjects
  type: array
- description: ''
  name: parameterObjects
  type: array
- description: ''
  name: parameterValues
  type: array
provider_name: Amazon Data Pipeline
provider_slug: amazon-data-pipeline
schema_file: json-schema/get-pipeline-definition-output-schema.json
slug: get-pipeline-definition-output
source_filename: get-pipeline-definition-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-pipeline/json-schema/get-pipeline-definition-output-schema.json\",\n  \"title\": \"Get Pipeline Definition Output\",\n  \"description\": \"Response containing the pipeline definition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineObjects\": {\n      \"type\": \"array\"\n    },\n    \"parameterObjects\": {\n      \"type\": \"array\"\n    },\n    \"parameterValues\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/json-schema/get-pipeline-definition-output-schema.json
tags:
- Data Processing
- ETL
- Workflows
- Data Pipeline
- Automation
title: Get Pipeline Definition Output
---
