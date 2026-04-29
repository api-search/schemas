---
description: Describes the configuration of an Auto Scaling group.
layout: schema
name: AutoScalingGroupConfiguration
properties_list:
- description: ''
  name: desiredCapacity
  type: object
- description: ''
  name: minSize
  type: object
- description: ''
  name: maxSize
  type: object
- description: ''
  name: instanceType
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-auto-scaling-group-configuration-schema.json
slug: compute-optimizer-auto-scaling-group-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-auto-scaling-group-configuration-schema.json\",\n  \"title\": \"AutoScalingGroupConfiguration\",\n  \"description\": \"Describes the configuration of an Auto Scaling group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"desiredCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DesiredCapacity\"\n        },\n        {\n          \"description\": \"The desired capacity, or number of instances, for the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"minSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MinSize\"\n        },\n        {\n          \"description\": \"The minimum size, or minimum number of instances, for the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"maxSize\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxSize\"\n        },\n        {\n          \"description\": \"The maximum size, or maximum number of instances, for the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"instanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceType\"\n        },\n        {\n          \"description\": \"The instance type for the Auto Scaling group.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-auto-scaling-group-configuration-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: AutoScalingGroupConfiguration
---
