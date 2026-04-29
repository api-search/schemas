---
description: The summary of a recommendation.
layout: schema
name: Summary
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: value
  type: object
- description: ''
  name: reasonCodeSummaries
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-summary-schema.json
slug: compute-optimizer-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-summary-schema.json\",\n  \"title\": \"Summary\",\n  \"description\": \"The summary of a recommendation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Finding\"\n        },\n        {\n          \"description\": \"The finding classification of the recommendation.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SummaryValue\"\n        },\n        {\n          \"description\": \"The value of the recommendation summary.\"\n        }\n      ]\n    },\n    \"reasonCodeSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReasonCodeSummaries\"\n        },\n        {\n          \"\
  description\": \"An array of objects that summarize a finding reason code.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-summary-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: Summary
---
