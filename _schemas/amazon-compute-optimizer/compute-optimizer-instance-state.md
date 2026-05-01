---
description: InstanceState schema
layout: schema
name: InstanceState
properties_list: []
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-instance-state-schema.json
slug: compute-optimizer-instance-state
source_filename: compute-optimizer-instance-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-instance-state-schema.json\",\n  \"title\": \"InstanceState\",\n  \"description\": \"InstanceState schema\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"pending\",\n    \"running\",\n    \"shutting-down\",\n    \"terminated\",\n    \"stopping\",\n    \"stopped\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-instance-state-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: InstanceState
---
