---
description: Complete pipeline export including all dependencies (sources, targets, connections, references, predictive models, geo fences, visualizations, and custom jars)
layout: schema
name: PipelineExport
properties_list:
- description: ''
  name: connections
  type: array
- description: ''
  name: references
  type: array
- description: ''
  name: customJars
  type: array
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-stream-analytics-rest-pipeline-export-schema.json
slug: oracle-goldengate-stream-analytics-rest-pipeline-export
source_filename: oracle-goldengate-stream-analytics-rest-pipeline-export-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PipelineExport\",\n  \"type\": \"object\",\n  \"description\": \"Complete pipeline export including all dependencies (sources, targets, connections, references, predictive models, geo fences, visualizations, and custom jars)\",\n  \"properties\": {\n    \"connections\": {\n      \"type\": \"array\"\n    },\n    \"references\": {\n      \"type\": \"array\"\n    },\n    \"customJars\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-stream-analytics-rest-pipeline-export-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: PipelineExport
---
