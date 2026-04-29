---
description: MetricName schema
layout: schema
name: MetricName
properties_list: []
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-metric-name-schema.json
slug: compute-optimizer-metric-name
source_filename: compute-optimizer-metric-name-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-metric-name-schema.json\",\n  \"title\": \"MetricName\",\n  \"description\": \"MetricName schema\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"Cpu\",\n    \"Memory\",\n    \"EBS_READ_OPS_PER_SECOND\",\n    \"EBS_WRITE_OPS_PER_SECOND\",\n    \"EBS_READ_BYTES_PER_SECOND\",\n    \"EBS_WRITE_BYTES_PER_SECOND\",\n    \"DISK_READ_OPS_PER_SECOND\",\n    \"DISK_WRITE_OPS_PER_SECOND\",\n    \"DISK_READ_BYTES_PER_SECOND\",\n    \"DISK_WRITE_BYTES_PER_SECOND\",\n    \"NETWORK_IN_BYTES_PER_SECOND\",\n    \"NETWORK_OUT_BYTES_PER_SECOND\",\n    \"NETWORK_PACKETS_IN_PER_SECOND\",\n    \"NETWORK_PACKETS_OUT_PER_SECOND\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-metric-name-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: MetricName
---
