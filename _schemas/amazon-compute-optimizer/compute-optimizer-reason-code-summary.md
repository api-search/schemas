---
description: A summary of a finding reason code.
layout: schema
name: ReasonCodeSummary
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-reason-code-summary-schema.json
slug: compute-optimizer-reason-code-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-reason-code-summary-schema.json\",\n  \"title\": \"ReasonCodeSummary\",\n  \"description\": \"A summary of a finding reason code.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingReasonCode\"\n        },\n        {\n          \"description\": \"The name of the finding reason code.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SummaryValue\"\n        },\n        {\n          \"description\": \"The value of the finding reason code summary.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-reason-code-summary-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: ReasonCodeSummary
---
