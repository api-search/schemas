---
description: GetRecommendationPreferencesRequest schema
layout: schema
name: GetRecommendationPreferencesRequest
properties_list:
- description: ''
  name: resourceType
  type: object
- description: ''
  name: scope
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-get-recommendation-preferences-request-schema.json
slug: compute-optimizer-get-recommendation-preferences-request
source_filename: compute-optimizer-get-recommendation-preferences-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-recommendation-preferences-request-schema.json\",\n  \"title\": \"GetRecommendationPreferencesRequest\",\n  \"description\": \"GetRecommendationPreferencesRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceType\"\n        },\n        {\n          \"description\": \"<p>The target resource type of the recommendation preference for which to return preferences.</p> <p>The <code>Ec2Instance</code> option encompasses standalone instances and instances that are part of Auto Scaling groups. The <code>AutoScalingGroup</code> option encompasses only instances that are part of an Auto Scaling group.</p> <note> <p>The valid values for this parameter are <code>Ec2Instance</code>\
  \ and <code>AutoScalingGroup</code>.</p> </note>\"\n        }\n      ]\n    },\n    \"scope\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scope\"\n        },\n        {\n          \"description\": \"<p>An object that describes the scope of the recommendation preference to return.</p> <p>You can return recommendation preferences that are created at the organization level (for management accounts of an organization only), account level, and resource level. For more information, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/enhanced-infrastructure-metrics.html\\\">Activating enhanced infrastructure metrics</a> in the <i>Compute Optimizer User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to advance to the next page of recommendation preferences.\"\n        }\n \
  \     ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"<p>The maximum number of recommendation preferences to return with a single request.</p> <p>To retrieve the remaining results, make another request with the returned <code>nextToken</code> value.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-recommendation-preferences-request-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: GetRecommendationPreferencesRequest
---
