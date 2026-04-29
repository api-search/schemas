---
description: Describes the recommendation preferences to return in the response of a <a>GetAutoScalingGroupRecommendations</a>, <a>GetEC2InstanceRecommendations</a>, and <a>GetEC2RecommendationProjectedMetrics</a> request.
layout: schema
name: RecommendationPreferences
properties_list:
- description: ''
  name: cpuVendorArchitectures
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-recommendation-preferences-schema.json
slug: compute-optimizer-recommendation-preferences
source_filename: compute-optimizer-recommendation-preferences-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-recommendation-preferences-schema.json\",\n  \"title\": \"RecommendationPreferences\",\n  \"description\": \"Describes the recommendation preferences to return in the response of a <a>GetAutoScalingGroupRecommendations</a>, <a>GetEC2InstanceRecommendations</a>, and <a>GetEC2RecommendationProjectedMetrics</a> request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cpuVendorArchitectures\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CpuVendorArchitectures\"\n        },\n        {\n          \"description\": \"<p>Specifies the CPU vendor and architecture for Amazon EC2 instance and Auto Scaling group recommendations.</p> <p>For example, when you specify <code>AWS_ARM64</code> with:</p> <ul> <li> <p>A <a>GetEC2InstanceRecommendations</a>\
  \ or <a>GetAutoScalingGroupRecommendations</a> request, Compute Optimizer returns recommendations that consist of Graviton2 instance types only.</p> </li> <li> <p>A <a>GetEC2RecommendationProjectedMetrics</a> request, Compute Optimizer returns projected utilization metrics for Graviton2 instance type recommendations only.</p> </li> <li> <p>A <a>ExportEC2InstanceRecommendations</a> or <a>ExportAutoScalingGroupRecommendations</a> request, Compute Optimizer exports recommendations that consist of Graviton2 instance types only.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-recommendation-preferences-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: RecommendationPreferences
---
