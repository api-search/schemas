---
description: GetEBSVolumeRecommendationsResponse schema
layout: schema
name: GetEBSVolumeRecommendationsResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: volumeRecommendations
  type: object
- description: ''
  name: errors
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-get-ebs-volume-recommendations-response-schema.json
slug: compute-optimizer-get-ebs-volume-recommendations-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-ebs-volume-recommendations-response-schema.json\",\n  \"title\": \"GetEBSVolumeRecommendationsResponse\",\n  \"description\": \"GetEBSVolumeRecommendationsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"<p>The token to use to advance to the next page of volume recommendations.</p> <p>This value is null when there are no more pages of volume recommendations to return.</p>\"\n        }\n      ]\n    },\n    \"volumeRecommendations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeRecommendations\"\n        },\n        {\n          \"description\": \"An array of objects\
  \ that describe volume recommendations.\"\n        }\n      ]\n    },\n    \"errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GetRecommendationErrors\"\n        },\n        {\n          \"description\": \"<p>An array of objects that describe errors of the request.</p> <p>For example, an error is returned if you request recommendations for an unsupported volume.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-ebs-volume-recommendations-response-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: GetEBSVolumeRecommendationsResponse
---
