---
description: The memory size configurations of a container.
layout: schema
name: MemorySizeConfiguration
properties_list:
- description: ''
  name: memory
  type: object
- description: ''
  name: memoryReservation
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-memory-size-configuration-schema.json
slug: compute-optimizer-memory-size-configuration
source_filename: compute-optimizer-memory-size-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-memory-size-configuration-schema.json\",\n  \"title\": \"MemorySizeConfiguration\",\n  \"description\": \" The memory size configurations of a container. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"memory\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableMemory\"\n        },\n        {\n          \"description\": \" The amount of memory in the container. \"\n        }\n      ]\n    },\n    \"memoryReservation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableMemoryReservation\"\n        },\n        {\n          \"description\": \" The limit of memory reserve for the container. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-memory-size-configuration-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: MemorySizeConfiguration
---
