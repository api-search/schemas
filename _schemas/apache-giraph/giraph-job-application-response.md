---
description: Single YARN application response
layout: schema
name: ApplicationResponse
properties_list:
- description: ''
  name: app
  type: object
provider_name: Apache Giraph
provider_slug: apache-giraph
schema_file: json-schema/giraph-job-application-response-schema.json
slug: giraph-job-application-response
source_filename: giraph-job-application-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-giraph/refs/heads/main/json-schema/giraph-job-application-response-schema.json\",\n  \"title\": \"ApplicationResponse\",\n  \"description\": \"Single YARN application response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"app\": {\n      \"$ref\": \"#/components/schemas/ApplicationInfo\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-giraph/refs/heads/main/json-schema/giraph-job-application-response-schema.json
tags:
- Apache
- Big Data
- BSP
- Graph Processing
- Hadoop
- Open Source
- Retired
title: ApplicationResponse
---
