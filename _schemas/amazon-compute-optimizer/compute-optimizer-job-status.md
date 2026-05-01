---
description: JobStatus schema
layout: schema
name: JobStatus
properties_list: []
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-job-status-schema.json
slug: compute-optimizer-job-status
source_filename: compute-optimizer-job-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-job-status-schema.json\",\n  \"title\": \"JobStatus\",\n  \"description\": \"JobStatus schema\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"Queued\",\n    \"InProgress\",\n    \"Complete\",\n    \"Failed\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-job-status-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: JobStatus
---
