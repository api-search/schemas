---
description: <p>Describes a filter that returns a more specific list of Amazon Elastic Block Store (Amazon EBS) volume recommendations. Use this filter with the <a>GetEBSVolumeRecommendations</a> action.</p> <p>You can use <code>LambdaFunctionRecommendationFilter</code> with the <a>GetLambdaFunctionRecommendations</a> action, <code>JobFilter</code> with the <a>DescribeRecommendationExportJobs</a> action, and <code>Filter</code> with the <a>GetAutoScalingGroupRecommendations</a> and <a>GetEC2InstanceRecommendations</a> actions.</p>
layout: schema
name: EBSFilter
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: values
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-ebs-filter-schema.json
slug: compute-optimizer-ebs-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-ebs-filter-schema.json\",\n  \"title\": \"EBSFilter\",\n  \"description\": \"<p>Describes a filter that returns a more specific list of Amazon Elastic Block Store (Amazon EBS) volume recommendations. Use this filter with the <a>GetEBSVolumeRecommendations</a> action.</p> <p>You can use <code>LambdaFunctionRecommendationFilter</code> with the <a>GetLambdaFunctionRecommendations</a> action, <code>JobFilter</code> with the <a>DescribeRecommendationExportJobs</a> action, and <code>Filter</code> with the <a>GetAutoScalingGroupRecommendations</a> and <a>GetEC2InstanceRecommendations</a> actions.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EBSFilterName\"\n        },\n        {\n   \
  \       \"description\": \"<p>The name of the filter.</p> <p>Specify <code>Finding</code> to return recommendations with a specific finding classification (for example, <code>NotOptimized</code>).</p> <p>You can filter your Amazon EBS volume recommendations by <code>tag:key</code> and <code>tag-key</code> tags.</p> <p>A <code>tag:key</code> is a key and value combination of a tag assigned to your Amazon EBS volume recommendations. Use the tag key in the filter name and the tag value as the filter value. For example, to find all Amazon EBS volume recommendations that have a tag with the key of <code>Owner</code> and the value of <code>TeamA</code>, specify <code>tag:Owner</code> for the filter name and <code>TeamA</code> for the filter value.</p> <p>A <code>tag-key</code> is the key of a tag assigned to your Amazon EBS volume recommendations. Use this filter to find all of your Amazon EBS volume recommendations that have a tag with a specific key. This doesn\\u2019t consider the tag value.\
  \ For example, you can find your Amazon EBS volume recommendations with a tag key value of <code>Owner</code> or without any tag keys assigned.</p>\"\n        }\n      ]\n    },\n    \"values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterValues\"\n        },\n        {\n          \"description\": \"<p>The value of the filter.</p> <p>The valid values are <code>Optimized</code>, or <code>NotOptimized</code>.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-ebs-filter-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: EBSFilter
---
