---
description: ''
layout: schema
name: ServiceHealth
properties_list:
- description: ''
  name: healthy
  type: boolean
- description: ''
  name: services
  type: array
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-big-data-rest-service-health-schema.json
slug: oracle-goldengate-big-data-rest-service-health
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceHealth\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"healthy\": {\n      \"type\": \"boolean\"\n    },\n    \"services\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-big-data-rest-service-health-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: ServiceHealth
---
