---
description: Describes an Amazon Elastic Block Store (Amazon EBS) volume recommendation.
layout: schema
name: VolumeRecommendation
properties_list:
- description: ''
  name: volumeArn
  type: object
- description: ''
  name: accountId
  type: object
- description: ''
  name: currentConfiguration
  type: object
- description: ''
  name: finding
  type: object
- description: ''
  name: utilizationMetrics
  type: object
- description: ''
  name: lookBackPeriodInDays
  type: object
- description: ''
  name: volumeRecommendationOptions
  type: object
- description: ''
  name: lastRefreshTimestamp
  type: object
- description: ''
  name: currentPerformanceRisk
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-volume-recommendation-schema.json
slug: compute-optimizer-volume-recommendation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-volume-recommendation-schema.json\",\n  \"title\": \"VolumeRecommendation\",\n  \"description\": \"Describes an Amazon Elastic Block Store (Amazon EBS) volume recommendation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"volumeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the current volume.\"\n        }\n      ]\n    },\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID of the volume.\"\n        }\n      ]\n    },\n    \"currentConfiguration\": {\n      \"allOf\": [\n        {\n        \
  \  \"$ref\": \"#/components/schemas/VolumeConfiguration\"\n        },\n        {\n          \"description\": \"An array of objects that describe the current configuration of the volume.\"\n        }\n      ]\n    },\n    \"finding\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EBSFinding\"\n        },\n        {\n          \"description\": \"<p>The finding classification of the volume.</p> <p>Findings for volumes include:</p> <ul> <li> <p> <b> <code>NotOptimized</code> </b>\\u2014A volume is considered not optimized when Compute Optimizer identifies a recommendation that can provide better performance for your workload.</p> </li> <li> <p> <b> <code>Optimized</code> </b>\\u2014An volume is considered optimized when Compute Optimizer determines that the volume is correctly provisioned to run your workload based on the chosen volume type. For optimized resources, Compute Optimizer might recommend a new generation volume type.</p> </li> </ul>\"\n        }\n\
  \      ]\n    },\n    \"utilizationMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EBSUtilizationMetrics\"\n        },\n        {\n          \"description\": \"An array of objects that describe the utilization metrics of the volume.\"\n        }\n      ]\n    },\n    \"lookBackPeriodInDays\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LookBackPeriodInDays\"\n        },\n        {\n          \"description\": \"The number of days for which utilization metrics were analyzed for the volume.\"\n        }\n      ]\n    },\n    \"volumeRecommendationOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeRecommendationOptions\"\n        },\n        {\n          \"description\": \"An array of objects that describe the recommendation options for the volume.\"\n        }\n      ]\n    },\n    \"lastRefreshTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastRefreshTimestamp\"\
  \n        },\n        {\n          \"description\": \"The timestamp of when the volume recommendation was last generated.\"\n        }\n      ]\n    },\n    \"currentPerformanceRisk\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CurrentPerformanceRisk\"\n        },\n        {\n          \"description\": \"The risk of the current EBS volume not meeting the performance needs of its workloads. The higher the risk, the more likely the current EBS volume doesn't have sufficient capacity.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \" A list of tags assigned to your Amazon EBS volume recommendations. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-volume-recommendation-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: VolumeRecommendation
---
