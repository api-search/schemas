---
description: DescribeRecommendationExportJobsRequest schema
layout: schema
name: DescribeRecommendationExportJobsRequest
properties_list:
- description: ''
  name: jobIds
  type: object
- description: ''
  name: filters
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-describe-recommendation-export-jobs-request-schema.json
slug: compute-optimizer-describe-recommendation-export-jobs-request
source_filename: compute-optimizer-describe-recommendation-export-jobs-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-describe-recommendation-export-jobs-request-schema.json\",\n  \"title\": \"DescribeRecommendationExportJobsRequest\",\n  \"description\": \"DescribeRecommendationExportJobsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobIds\"\n        },\n        {\n          \"description\": \"<p>The identification numbers of the export jobs to return.</p> <p>An export job ID is returned when you create an export using the <a>ExportAutoScalingGroupRecommendations</a> or <a>ExportEC2InstanceRecommendations</a> actions.</p> <p>All export jobs created in the last seven days are returned if this parameter is omitted.</p>\"\n        }\n      ]\n    },\n    \"filters\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/JobFilters\"\n        },\n        {\n          \"description\": \"An array of objects to specify a filter that returns a more specific list of export jobs.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to advance to the next page of export jobs.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"<p>The maximum number of export jobs to return with a single request.</p> <p>To retrieve the remaining results, make another request with the returned <code>nextToken</code> value.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-describe-recommendation-export-jobs-request-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: DescribeRecommendationExportJobsRequest
---
