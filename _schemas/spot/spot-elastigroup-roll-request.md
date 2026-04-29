---
description: ''
layout: schema
name: RollRequest
properties_list:
- description: Percentage of instances to replace in each batch.
  name: batchSizePercentage
  type: integer
- description: Grace period in seconds before checking health.
  name: gracePeriod
  type: integer
- description: ''
  name: healthCheckType
  type: string
provider_name: Spot
provider_slug: spot
schema_file: json-schema/spot-elastigroup-roll-request-schema.json
slug: spot-elastigroup-roll-request
source_filename: spot-elastigroup-roll-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RollRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"batchSizePercentage\": {\n      \"type\": \"integer\",\n      \"description\": \"Percentage of instances to replace in each batch.\"\n    },\n    \"gracePeriod\": {\n      \"type\": \"integer\",\n      \"description\": \"Grace period in seconds before checking health.\"\n    },\n    \"healthCheckType\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/json-schema/spot-elastigroup-roll-request-schema.json
tags:
- Autoscaling
- Cloud Infrastructure
- Containers
- Cost Optimization
- FinOps
- Kubernetes
- Spot Instances
title: RollRequest
---
