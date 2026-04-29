---
description: Response containing a list of pipeline identifiers.
layout: schema
name: List Pipelines Output
properties_list:
- description: ''
  name: pipelineIdList
  type: array
- description: ''
  name: hasMoreResults
  type: boolean
- description: ''
  name: marker
  type: string
provider_name: Amazon Data Pipeline
provider_slug: amazon-data-pipeline
schema_file: json-schema/list-pipelines-output-schema.json
slug: list-pipelines-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-pipeline/json-schema/list-pipelines-output-schema.json\",\n  \"title\": \"List Pipelines Output\",\n  \"description\": \"Response containing a list of pipeline identifiers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineIdList\": {\n      \"type\": \"array\"\n    },\n    \"hasMoreResults\": {\n      \"type\": \"boolean\"\n    },\n    \"marker\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/json-schema/list-pipelines-output-schema.json
tags:
- AWS
- Data Processing
- ETL
- Workflows
- Data Pipeline
- Automation
title: List Pipelines Output
---
