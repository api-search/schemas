---
description: ''
layout: schema
name: UpdateServerConfigurationRequest
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
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-veridata-rest-update-server-configuration-request-schema.json
slug: oracle-goldengate-veridata-rest-update-server-configuration-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateServerConfigurationRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxConcurrentJobs\": {\n      \"type\": \"integer\"\n    },\n    \"maxThreadsPerJob\": {\n      \"type\": \"integer\"\n    },\n    \"reportRetentionDays\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-veridata-rest-update-server-configuration-request-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: UpdateServerConfigurationRequest
---
