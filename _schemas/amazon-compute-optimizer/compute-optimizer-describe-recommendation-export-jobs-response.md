---
description: DescribeRecommendationExportJobsResponse schema
layout: schema
name: DescribeRecommendationExportJobsResponse
properties_list:
- description: ''
  name: recommendationExportJobs
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-describe-recommendation-export-jobs-response-schema.json
slug: compute-optimizer-describe-recommendation-export-jobs-response
source_filename: compute-optimizer-describe-recommendation-export-jobs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-describe-recommendation-export-jobs-response-schema.json\",\n  \"title\": \"DescribeRecommendationExportJobsResponse\",\n  \"description\": \"DescribeRecommendationExportJobsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"recommendationExportJobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendationExportJobs\"\n        },\n        {\n          \"description\": \"An array of objects that describe recommendation export jobs.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"<p>The token to use to advance to the next page of export jobs.</p> <p>This value is null when there\
  \ are no more pages of export jobs to return.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-describe-recommendation-export-jobs-response-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: DescribeRecommendationExportJobsResponse
---
