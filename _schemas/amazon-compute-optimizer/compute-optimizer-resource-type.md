---
description: ResourceType schema
layout: schema
name: ResourceType
properties_list: []
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-resource-type-schema.json
slug: compute-optimizer-resource-type
source_filename: compute-optimizer-resource-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-resource-type-schema.json\",\n  \"title\": \"ResourceType\",\n  \"description\": \"ResourceType schema\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"Ec2Instance\",\n    \"AutoScalingGroup\",\n    \"EbsVolume\",\n    \"LambdaFunction\",\n    \"NotApplicable\",\n    \"EcsService\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-resource-type-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: ResourceType
---
