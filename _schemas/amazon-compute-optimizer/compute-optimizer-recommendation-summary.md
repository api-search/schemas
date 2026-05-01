---
description: A summary of a recommendation.
layout: schema
name: RecommendationSummary
properties_list:
- description: ''
  name: summaries
  type: object
- description: ''
  name: recommendationResourceType
  type: object
- description: ''
  name: accountId
  type: object
- description: ''
  name: savingsOpportunity
  type: object
- description: ''
  name: currentPerformanceRiskRatings
  type: object
- description: ''
  name: inferredWorkloadSavings
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-recommendation-summary-schema.json
slug: compute-optimizer-recommendation-summary
source_filename: compute-optimizer-recommendation-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-recommendation-summary-schema.json\",\n  \"title\": \"RecommendationSummary\",\n  \"description\": \"A summary of a recommendation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"summaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Summaries\"\n        },\n        {\n          \"description\": \"An array of objects that describe a recommendation summary.\"\n        }\n      ]\n    },\n    \"recommendationResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendationSourceType\"\n        },\n        {\n          \"description\": \"The resource type that the recommendation summary applies to.\"\n        }\n      ]\n    },\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID of the recommendation summary.\"\n        }\n      ]\n    },\n    \"savingsOpportunity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SavingsOpportunity\"\n        },\n        {\n          \"description\": \"An object that describes the savings opportunity for a given resource type. Savings opportunity includes the estimated monthly savings amount and percentage.\"\n        }\n      ]\n    },\n    \"currentPerformanceRiskRatings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CurrentPerformanceRiskRatings\"\n        },\n        {\n          \"description\": \"An object that describes the performance risk ratings for a given resource type.\"\n        }\n      ]\n    },\n    \"inferredWorkloadSavings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InferredWorkloadSavings\"\
  \n        },\n        {\n          \"description\": \" An array of objects that describes the estimated monthly saving amounts for the instances running on the specified <code>inferredWorkloadTypes</code>. The array contains the top three savings opportunites for the instances running inferred workload types. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-recommendation-summary-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: RecommendationSummary
---
