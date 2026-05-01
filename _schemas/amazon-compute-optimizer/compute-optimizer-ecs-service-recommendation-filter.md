---
description: Describes a filter that returns a more specific list of Amazon ECS service recommendations. Use this filter with the <a>GetECSServiceRecommendations</a> action.
layout: schema
name: ECSServiceRecommendationFilter
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: values
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-ecs-service-recommendation-filter-schema.json
slug: compute-optimizer-ecs-service-recommendation-filter
source_filename: compute-optimizer-ecs-service-recommendation-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-ecs-service-recommendation-filter-schema.json\",\n  \"title\": \"ECSServiceRecommendationFilter\",\n  \"description\": \" Describes a filter that returns a more specific list of Amazon ECS service recommendations. Use this filter with the <a>GetECSServiceRecommendations</a> action. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSServiceRecommendationFilterName\"\n        },\n        {\n          \"description\": \"<p> The name of the filter. </p> <p> Specify <code>Finding</code> to return recommendations with a specific finding classification. </p> <p> Specify <code>FindingReasonCode</code> to return recommendations with a specific finding reason code. </p> <p>You can filter your\
  \ Amazon ECS service recommendations by <code>tag:key</code> and <code>tag-key</code> tags.</p> <p>A <code>tag:key</code> is a key and value combination of a tag assigned to your Amazon ECS service recommendations. Use the tag key in the filter name and the tag value as the filter value. For example, to find all Amazon ECS service recommendations that have a tag with the key of <code>Owner</code> and the value of <code>TeamA</code>, specify <code>tag:Owner</code> for the filter name and <code>TeamA</code> for the filter value.</p> <p>A <code>tag-key</code> is the key of a tag assigned to your Amazon ECS service recommendations. Use this filter to find all of your Amazon ECS service recommendations that have a tag with a specific key. This doesn\\u2019t consider the tag value. For example, you can find your Amazon ECS service recommendations with a tag key value of <code>Owner</code> or without any tag keys assigned.</p>\"\n        }\n      ]\n    },\n    \"values\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/FilterValues\"\n        },\n        {\n          \"description\": \"<p> The value of the filter. </p> <p>The valid values for this parameter are as follows:</p> <ul> <li> <p>If you specify the <code>name</code> parameter as <code>Finding</code>, specify <code>Optimized</code>, <code>NotOptimized</code>, or <code>Unavailable</code>.</p> </li> <li> <p>If you specify the <code>name</code> parameter as <code>FindingReasonCode</code>, specify <code>CPUUnderprovisioned</code>, <code>CPUOverprovisioned</code>, <code>MemoryUnderprovisioned</code>, or <code>MemoryOverprovisioned</code>.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-ecs-service-recommendation-filter-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: ECSServiceRecommendationFilter
---
