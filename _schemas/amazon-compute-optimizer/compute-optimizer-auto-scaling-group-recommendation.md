---
description: Describes an Auto Scaling group recommendation.
layout: schema
name: AutoScalingGroupRecommendation
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: autoScalingGroupArn
  type: object
- description: ''
  name: autoScalingGroupName
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
  name: currentConfiguration
  type: object
- description: ''
  name: recommendationOptions
  type: object
- description: ''
  name: lastRefreshTimestamp
  type: object
- description: ''
  name: currentPerformanceRisk
  type: object
- description: ''
  name: effectiveRecommendationPreferences
  type: object
- description: ''
  name: inferredWorkloadTypes
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-auto-scaling-group-recommendation-schema.json
slug: compute-optimizer-auto-scaling-group-recommendation
source_filename: compute-optimizer-auto-scaling-group-recommendation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-auto-scaling-group-recommendation-schema.json\",\n  \"title\": \"AutoScalingGroupRecommendation\",\n  \"description\": \"Describes an Auto Scaling group recommendation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"autoScalingGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"autoScalingGroupName\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupName\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"finding\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Finding\"\n        },\n        {\n          \"description\": \"<p>The finding classification of the Auto Scaling group.</p> <p>Findings for Auto Scaling groups include:</p> <ul> <li> <p> <b> <code>NotOptimized</code> </b>\\u2014An Auto Scaling group is considered not optimized when Compute Optimizer identifies a recommendation that can provide better performance for your workload.</p> </li> <li> <p> <b> <code>Optimized</code> </b>\\u2014An Auto Scaling group is considered optimized when Compute Optimizer determines that the group is correctly provisioned to run your workload based on the chosen instance type. For optimized resources, Compute Optimizer might recommend a new generation instance type.</p>\
  \ </li> </ul>\"\n        }\n      ]\n    },\n    \"utilizationMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UtilizationMetrics\"\n        },\n        {\n          \"description\": \"An array of objects that describe the utilization metrics of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"lookBackPeriodInDays\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LookBackPeriodInDays\"\n        },\n        {\n          \"description\": \"The number of days for which utilization metrics were analyzed for the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"currentConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupConfiguration\"\n        },\n        {\n          \"description\": \"An array of objects that describe the current configuration of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"recommendationOptions\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupRecommendationOptions\"\n        },\n        {\n          \"description\": \"An array of objects that describe the recommendation options for the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"lastRefreshTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastRefreshTimestamp\"\n        },\n        {\n          \"description\": \"The timestamp of when the Auto Scaling group recommendation was last generated.\"\n        }\n      ]\n    },\n    \"currentPerformanceRisk\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CurrentPerformanceRisk\"\n        },\n        {\n          \"description\": \"The risk of the current Auto Scaling group not meeting the performance needs of its workloads. The higher the risk, the more likely the current Auto Scaling group configuration has insufficient capacity and cannot meet workload requirements.\"\n \
  \       }\n      ]\n    },\n    \"effectiveRecommendationPreferences\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EffectiveRecommendationPreferences\"\n        },\n        {\n          \"description\": \"An object that describes the effective recommendation preferences for the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"inferredWorkloadTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InferredWorkloadTypes\"\n        },\n        {\n          \"description\": \"<p>The applications that might be running on the instances in the Auto Scaling group as inferred by Compute Optimizer.</p> <p>Compute Optimizer can infer if one of the following applications might be running on the instances:</p> <ul> <li> <p> <code>AmazonEmr</code> - Infers that Amazon EMR might be running on the instances.</p> </li> <li> <p> <code>ApacheCassandra</code> - Infers that Apache Cassandra might be running on the instances.</p> </li>\
  \ <li> <p> <code>ApacheHadoop</code> - Infers that Apache Hadoop might be running on the instances.</p> </li> <li> <p> <code>Memcached</code> - Infers that Memcached might be running on the instances.</p> </li> <li> <p> <code>NGINX</code> - Infers that NGINX might be running on the instances.</p> </li> <li> <p> <code>PostgreSql</code> - Infers that PostgreSQL might be running on the instances.</p> </li> <li> <p> <code>Redis</code> - Infers that Redis might be running on the instances.</p> </li> <li> <p> <code>Kafka</code> - Infers that Kafka might be running on the instance.</p> </li> <li> <p> <code>SQLServer</code> - Infers that SQLServer might be running on the instance.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-auto-scaling-group-recommendation-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: AutoScalingGroupRecommendation
---
