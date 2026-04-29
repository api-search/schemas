---
description: YARN applications list response
layout: schema
name: ApplicationsResponse
properties_list:
- description: Applications wrapper
  name: apps
  type: object
provider_name: Apache Giraph
provider_slug: apache-giraph
schema_file: json-schema/giraph-job-applications-response-schema.json
slug: giraph-job-applications-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-giraph/refs/heads/main/json-schema/giraph-job-applications-response-schema.json\",\n  \"title\": \"ApplicationsResponse\",\n  \"description\": \"YARN applications list response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apps\": {\n      \"type\": \"object\",\n      \"description\": \"Applications wrapper\",\n      \"properties\": {\n        \"app\": {\n          \"type\": \"array\",\n          \"description\": \"List of application entries\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/ApplicationInfo\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-giraph/refs/heads/main/json-schema/giraph-job-applications-response-schema.json
tags:
- Apache
- Big Data
- BSP
- Graph Processing
- Hadoop
- Open Source
- Retired
title: ApplicationsResponse
---
