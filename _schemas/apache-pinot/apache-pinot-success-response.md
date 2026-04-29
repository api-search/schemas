---
description: SuccessResponse schema from Apache Pinot
layout: schema
name: SuccessResponse
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: message
  type: string
provider_name: Apache Pinot
provider_slug: apache-pinot
schema_file: json-schema/apache-pinot-success-response-schema.json
slug: apache-pinot-success-response
source_filename: apache-pinot-success-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-success-response-schema.json\",\n  \"title\": \"SuccessResponse\",\n  \"description\": \"SuccessResponse schema from Apache Pinot\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"success\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"example\": \"Table created successfully\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-success-response-schema.json
tags:
- Analytics
- Database
- Low Latency
- OLAP
- Real-Time
- Apache
- Open Source
title: SuccessResponse
---
