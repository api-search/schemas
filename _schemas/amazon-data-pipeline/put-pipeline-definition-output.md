---
description: Response after updating the pipeline definition.
layout: schema
name: Put Pipeline Definition Output
properties_list:
- description: ''
  name: errored
  type: boolean
- description: ''
  name: validationErrors
  type: array
- description: ''
  name: validationWarnings
  type: array
provider_name: Amazon Data Pipeline
provider_slug: amazon-data-pipeline
schema_file: json-schema/put-pipeline-definition-output-schema.json
slug: put-pipeline-definition-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-pipeline/json-schema/put-pipeline-definition-output-schema.json\",\n  \"title\": \"Put Pipeline Definition Output\",\n  \"description\": \"Response after updating the pipeline definition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errored\": {\n      \"type\": \"boolean\"\n    },\n    \"validationErrors\": {\n      \"type\": \"array\"\n    },\n    \"validationWarnings\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/json-schema/put-pipeline-definition-output-schema.json
tags:
- AWS
- Data Processing
- ETL
- Workflows
- Data Pipeline
- Automation
title: Put Pipeline Definition Output
---
