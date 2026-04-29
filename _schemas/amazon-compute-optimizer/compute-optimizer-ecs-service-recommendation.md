---
description: Describes an Amazon ECS service recommendation.
layout: schema
name: ECSServiceRecommendation
properties_list:
- description: ''
  name: serviceArn
  type: object
- description: ''
  name: accountId
  type: object
- description: ''
  name: currentServiceConfiguration
  type: object
- description: ''
  name: utilizationMetrics
  type: object
- description: ''
  name: lookbackPeriodInDays
  type: object
- description: ''
  name: launchType
  type: object
- description: ''
  name: lastRefreshTimestamp
  type: object
- description: ''
  name: finding
  type: object
- description: ''
  name: findingReasonCodes
  type: object
- description: ''
  name: serviceRecommendationOptions
  type: object
- description: ''
  name: currentPerformanceRisk
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-ecs-service-recommendation-schema.json
slug: compute-optimizer-ecs-service-recommendation
source_filename: compute-optimizer-ecs-service-recommendation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-ecs-service-recommendation-schema.json\",\n  \"title\": \"ECSServiceRecommendation\",\n  \"description\": \" Describes an Amazon ECS service recommendation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceArn\"\n        },\n        {\n          \"description\": \"<p> The Amazon Resource Name (ARN) of the current Amazon ECS service. </p> <p> The following is the format of the ARN: </p> <p> <code>arn:aws:ecs:region:aws_account_id:service/cluster-name/service-name</code> </p>\"\n        }\n      ]\n    },\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \" The Amazon\
  \ Web Services account ID of the Amazon ECS service. \"\n        }\n      ]\n    },\n    \"currentServiceConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceConfiguration\"\n        },\n        {\n          \"description\": \" The configuration of the current Amazon ECS service. \"\n        }\n      ]\n    },\n    \"utilizationMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSServiceUtilizationMetrics\"\n        },\n        {\n          \"description\": \" An array of objects that describe the utilization metrics of the Amazon ECS service. \"\n        }\n      ]\n    },\n    \"lookbackPeriodInDays\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LookBackPeriodInDays\"\n        },\n        {\n          \"description\": \" The number of days the Amazon ECS service utilization metrics were analyzed. \"\n        }\n      ]\n    },\n    \"launchType\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/ECSServiceLaunchType\"\n        },\n        {\n          \"description\": \"<p> The launch type the Amazon ECS service is using. </p> <note> <p>Compute Optimizer only supports the Fargate launch type.</p> </note>\"\n        }\n      ]\n    },\n    \"lastRefreshTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastRefreshTimestamp\"\n        },\n        {\n          \"description\": \" The timestamp of when the Amazon ECS service recommendation was last generated. \"\n        }\n      ]\n    },\n    \"finding\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSServiceRecommendationFinding\"\n        },\n        {\n          \"description\": \"<p> The finding classification of an Amazon ECS service. </p> <p>Findings for Amazon ECS services include:</p> <ul> <li> <p> <b> <code>Underprovisioned</code> </b> \\u2014 When Compute Optimizer detects that there\\u2019s\
  \ not enough memory or CPU, an Amazon ECS service is considered under-provisioned. An under-provisioned service might result in poor application performance.</p> </li> <li> <p> <b> <code>Overprovisioned</code> </b> \\u2014 When Compute Optimizer detects that there\\u2019s excessive memory or CPU, an Amazon ECS service is considered over-provisioned. An over-provisioned service might result in additional infrastructure costs. </p> </li> <li> <p> <b> <code>Optimized</code> </b> \\u2014 When both the CPU and memory of your Amazon ECS service meet the performance requirements of your workload, the service is considered optimized.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"findingReasonCodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSServiceRecommendationFindingReasonCodes\"\n        },\n        {\n          \"description\": \"<p> The reason for the finding classification of an Amazon ECS service. </p> <p>Finding reason codes for Amazon ECS\
  \ services include:</p> <ul> <li> <p> <b> <code>CPUUnderprovisioned</code> </b> \\u2014 The service CPU configuration can be sized up to enhance the performance of your workload. This is identified by analyzing the <code>CPUUtilization</code> metric of the current service during the look-back period.</p> </li> <li> <p> <b> <code>CPUOverprovisioned</code> </b> \\u2014 The service CPU configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the <code>CPUUtilization</code> metric of the current service during the look-back period. </p> </li> <li> <p> <b> <code>MemoryUnderprovisioned</code> </b> \\u2014 The service memory configuration can be sized up to enhance the performance of your workload. This is identified by analyzing the <code>MemoryUtilization</code> metric of the current service during the look-back period.</p> </li> <li> <p> <b> <code>MemoryOverprovisioned</code> </b> \\u2014 The service memory configuration\
  \ can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the <code>MemoryUtilization</code> metric of the current service during the look-back period.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"serviceRecommendationOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSServiceRecommendationOptions\"\n        },\n        {\n          \"description\": \" An array of objects that describe the recommendation options for the Amazon ECS service. \"\n        }\n      ]\n    },\n    \"currentPerformanceRisk\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CurrentPerformanceRisk\"\n        },\n        {\n          \"description\": \" The risk of the current Amazon ECS service not meeting the performance needs of its workloads. The higher the risk, the more likely the current service can't meet the performance requirements of its workload. \"\n        }\n   \
  \   ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \" A list of tags assigned to your Amazon ECS service recommendations. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-ecs-service-recommendation-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: ECSServiceRecommendation
---
