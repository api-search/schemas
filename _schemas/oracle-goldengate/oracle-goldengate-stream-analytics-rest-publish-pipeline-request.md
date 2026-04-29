---
description: ''
layout: schema
name: PublishPipelineRequest
properties_list:
- description: Optional Spark configuration overrides
  name: sparkConfig
  type: object
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-stream-analytics-rest-publish-pipeline-request-schema.json
slug: oracle-goldengate-stream-analytics-rest-publish-pipeline-request
source_filename: oracle-goldengate-stream-analytics-rest-publish-pipeline-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PublishPipelineRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sparkConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Optional Spark configuration overrides\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-stream-analytics-rest-publish-pipeline-request-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: PublishPipelineRequest
---
