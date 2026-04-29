---
description: <p>Describes the performance risk ratings for a given resource type.</p> <p>Resources with a <code>high</code> or <code>medium</code> rating are at risk of not meeting the performance needs of their workloads, while resources with a <code>low</code> rating are performing well in their workloads.</p>
layout: schema
name: CurrentPerformanceRiskRatings
properties_list:
- description: ''
  name: high
  type: object
- description: ''
  name: medium
  type: object
- description: ''
  name: low
  type: object
- description: ''
  name: veryLow
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-current-performance-risk-ratings-schema.json
slug: compute-optimizer-current-performance-risk-ratings
source_filename: compute-optimizer-current-performance-risk-ratings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-current-performance-risk-ratings-schema.json\",\n  \"title\": \"CurrentPerformanceRiskRatings\",\n  \"description\": \"<p>Describes the performance risk ratings for a given resource type.</p> <p>Resources with a <code>high</code> or <code>medium</code> rating are at risk of not meeting the performance needs of their workloads, while resources with a <code>low</code> rating are performing well in their workloads.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"high\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/High\"\n        },\n        {\n          \"description\": \"A count of the applicable resource types with a high performance risk rating.\"\n        }\n      ]\n    },\n    \"medium\": {\n      \"allOf\": [\n        {\n     \
  \     \"$ref\": \"#/components/schemas/Medium\"\n        },\n        {\n          \"description\": \"A count of the applicable resource types with a medium performance risk rating.\"\n        }\n      ]\n    },\n    \"low\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Low\"\n        },\n        {\n          \"description\": \"A count of the applicable resource types with a low performance risk rating.\"\n        }\n      ]\n    },\n    \"veryLow\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VeryLow\"\n        },\n        {\n          \"description\": \"A count of the applicable resource types with a very low performance risk rating.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-current-performance-risk-ratings-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: CurrentPerformanceRiskRatings
---
