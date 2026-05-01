---
description: <p>Describes a filter that returns a more specific list of Lambda function recommendations. Use this filter with the <a>GetLambdaFunctionRecommendations</a> action.</p> <p>You can use <code>EBSFilter</code> with the <a>GetEBSVolumeRecommendations</a> action, <code>JobFilter</code> with the <a>DescribeRecommendationExportJobs</a> action, and <code>Filter</code> with the <a>GetAutoScalingGroupRecommendations</a> and <a>GetEC2InstanceRecommendations</a> actions.</p>
layout: schema
name: LambdaFunctionRecommendationFilter
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: values
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-lambda-function-recommendation-filter-schema.json
slug: compute-optimizer-lambda-function-recommendation-filter
source_filename: compute-optimizer-lambda-function-recommendation-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-lambda-function-recommendation-filter-schema.json\",\n  \"title\": \"LambdaFunctionRecommendationFilter\",\n  \"description\": \"<p>Describes a filter that returns a more specific list of Lambda function recommendations. Use this filter with the <a>GetLambdaFunctionRecommendations</a> action.</p> <p>You can use <code>EBSFilter</code> with the <a>GetEBSVolumeRecommendations</a> action, <code>JobFilter</code> with the <a>DescribeRecommendationExportJobs</a> action, and <code>Filter</code> with the <a>GetAutoScalingGroupRecommendations</a> and <a>GetEC2InstanceRecommendations</a> actions.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionRecommendationFilterName\"\n     \
  \   },\n        {\n          \"description\": \"<p>The name of the filter.</p> <p>Specify <code>Finding</code> to return recommendations with a specific finding classification (for example, <code>NotOptimized</code>).</p> <p>Specify <code>FindingReasonCode</code> to return recommendations with a specific finding reason code (for example, <code>MemoryUnderprovisioned</code>).</p> <p>You can filter your Lambda function recommendations by <code>tag:key</code> and <code>tag-key</code> tags.</p> <p>A <code>tag:key</code> is a key and value combination of a tag assigned to your Lambda function recommendations. Use the tag key in the filter name and the tag value as the filter value. For example, to find all Lambda function recommendations that have a tag with the key of <code>Owner</code> and the value of <code>TeamA</code>, specify <code>tag:Owner</code> for the filter name and <code>TeamA</code> for the filter value.</p> <p>A <code>tag-key</code> is the key of a tag assigned to your Lambda\
  \ function recommendations. Use this filter to find all of your Lambda function recommendations that have a tag with a specific key. This doesn\\u2019t consider the tag value. For example, you can find your Lambda function recommendations with a tag key value of <code>Owner</code> or without any tag keys assigned.</p>\"\n        }\n      ]\n    },\n    \"values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterValues\"\n        },\n        {\n          \"description\": \"<p>The value of the filter.</p> <p>The valid values for this parameter are as follows, depending on what you specify for the <code>name</code> parameter:</p> <ul> <li> <p>Specify <code>Optimized</code>, <code>NotOptimized</code>, or <code>Unavailable</code> if you specify the <code>name</code> parameter as <code>Finding</code>.</p> </li> <li> <p>Specify <code>MemoryOverprovisioned</code>, <code>MemoryUnderprovisioned</code>, <code>InsufficientData</code>, or <code>Inconclusive</code>\
  \ if you specify the <code>name</code> parameter as <code>FindingReasonCode</code>.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-lambda-function-recommendation-filter-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: LambdaFunctionRecommendationFilter
---
