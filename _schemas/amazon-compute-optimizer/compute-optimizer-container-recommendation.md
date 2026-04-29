---
description: The CPU and memory recommendations for a container within the tasks of your Amazon ECS service.
layout: schema
name: ContainerRecommendation
properties_list:
- description: ''
  name: containerName
  type: object
- description: ''
  name: memorySizeConfiguration
  type: object
- description: ''
  name: cpu
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-container-recommendation-schema.json
slug: compute-optimizer-container-recommendation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-container-recommendation-schema.json\",\n  \"title\": \"ContainerRecommendation\",\n  \"description\": \" The CPU and memory recommendations for a container within the tasks of your Amazon ECS service. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"containerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerName\"\n        },\n        {\n          \"description\": \" The name of the container. \"\n        }\n      ]\n    },\n    \"memorySizeConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemorySizeConfiguration\"\n        },\n        {\n          \"description\": \" The recommended memory size configurations for the container. \"\n        }\n      ]\n    },\n    \"cpu\": {\n   \
  \   \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableCpu\"\n        },\n        {\n          \"description\": \" The recommended number of CPU units reserved for the container. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-container-recommendation-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: ContainerRecommendation
---
