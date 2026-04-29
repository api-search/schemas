---
description: ''
layout: schema
name: ServerConfiguration
properties_list:
- description: ''
  name: maxConcurrentJobs
  type: integer
- description: ''
  name: maxThreadsPerJob
  type: integer
- description: ''
  name: reportRetentionDays
  type: integer
- description: ''
  name: oosRetentionDays
  type: integer
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-veridata-rest-server-configuration-schema.json
slug: oracle-goldengate-veridata-rest-server-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServerConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxConcurrentJobs\": {\n      \"type\": \"integer\"\n    },\n    \"maxThreadsPerJob\": {\n      \"type\": \"integer\"\n    },\n    \"reportRetentionDays\": {\n      \"type\": \"integer\"\n    },\n    \"oosRetentionDays\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-veridata-rest-server-configuration-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: ServerConfiguration
---
