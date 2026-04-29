---
description: Information about global partition states.
layout: schema
name: GlobalPartitionStatesResponse
properties_list:
- description: ''
  name: states
  type: array
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-global-partition-states-response-schema.json
slug: rest-api-global-partition-states-response
source_filename: rest-api-global-partition-states-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-global-partition-states-response-schema.json\",\n  \"title\": \"GlobalPartitionStatesResponse\",\n  \"description\": \"Information about global partition states.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"states\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/GlobalPartitionStateResponse\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-global-partition-states-response-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: GlobalPartitionStatesResponse
---
