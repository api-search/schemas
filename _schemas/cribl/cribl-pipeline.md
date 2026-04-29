---
description: A Cribl processing pipeline that defines an ordered sequence of functions for transforming, filtering, and enriching observability data events in real time.
layout: schema
name: Cribl Pipeline
properties_list:
- description: Unique identifier for the pipeline
  name: id
  type: string
- description: Pipeline configuration containing functions and settings
  name: conf
  type: object
provider_name: Cribl
provider_slug: cribl
schema_file: json-schema/cribl-pipeline-schema.json
slug: cribl-pipeline
source_filename: cribl-pipeline-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.cribl.io/schemas/cribl/pipeline.json\",\n  \"title\": \"Cribl Pipeline\",\n  \"description\": \"A Cribl processing pipeline that defines an ordered sequence of functions for transforming, filtering, and enriching observability data events in real time.\",\n  \"type\": \"object\",\n  \"required\": [\"id\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the pipeline\",\n      \"pattern\": \"^[a-zA-Z0-9_-]+$\"\n    },\n    \"conf\": {\n      \"type\": \"object\",\n      \"description\": \"Pipeline configuration containing functions and settings\",\n      \"properties\": {\n        \"functions\": {\n          \"type\": \"array\",\n          \"description\": \"Ordered list of processing functions that events pass through sequentially\",\n          \"items\": {\n            \"$ref\": \"#/$defs/PipelineFunction\"\n   \
  \       }\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A human-readable description of the pipeline purpose\"\n        },\n        \"asyncFuncTimeout\": {\n          \"type\": \"integer\",\n          \"description\": \"Timeout for asynchronous functions in milliseconds\",\n          \"minimum\": 0,\n          \"maximum\": 300000\n        },\n        \"output\": {\n          \"type\": \"string\",\n          \"description\": \"Default output destination for processed events\"\n        },\n        \"streamtags\": {\n          \"type\": \"array\",\n          \"description\": \"Tags applied to all events processed by this pipeline\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"groups\": {\n          \"type\": \"object\",\n          \"description\": \"Worker group or fleet-specific configuration overrides\",\n          \"additionalProperties\": {\n            \"type\": \"object\",\n  \
  \          \"description\": \"Group-specific pipeline settings\"\n          }\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"PipelineFunction\": {\n      \"type\": \"object\",\n      \"description\": \"A processing function within a pipeline that performs a specific data transformation operation.\",\n      \"required\": [\"id\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The function type identifier such as eval, regex_extract, rename, mask, aggregate, or serialize\"\n        },\n        \"filter\": {\n          \"type\": \"string\",\n          \"description\": \"JavaScript expression that determines which events this function processes. Returns true to process, false to skip.\"\n        },\n        \"disabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this function is disabled and should be skipped during processing\",\n          \"default\": false\n        },\n        \"conf\"\
  : {\n          \"type\": \"object\",\n          \"description\": \"Function-specific configuration parameters that vary by function type\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A human-readable description of what this function does\"\n        },\n        \"final\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to stop processing subsequent functions after this one\",\n          \"default\": false\n        },\n        \"groupId\": {\n          \"type\": \"string\",\n          \"description\": \"Group identifier for visually grouping functions in the UI\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cribl/refs/heads/main/json-schema/cribl-pipeline-schema.json
tags:
- Configuration
- Data Lake
- Data Pipelines
- Data Routing
- Edge Computing
- Infrastructure as Code
- Observability
- Search
- Security Data
- Stream Processing
- Telemetry
title: Cribl Pipeline
---
