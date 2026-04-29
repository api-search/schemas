---
description: The Amazon ECS service configurations used for recommendations.
layout: schema
name: ServiceConfiguration
properties_list:
- description: ''
  name: memory
  type: object
- description: ''
  name: cpu
  type: object
- description: ''
  name: containerConfigurations
  type: object
- description: ''
  name: autoScalingConfiguration
  type: object
- description: ''
  name: taskDefinitionArn
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-service-configuration-schema.json
slug: compute-optimizer-service-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-service-configuration-schema.json\",\n  \"title\": \"ServiceConfiguration\",\n  \"description\": \" The Amazon ECS service configurations used for recommendations. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"memory\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableMemory\"\n        },\n        {\n          \"description\": \" The amount of memory used by the tasks in the Amazon ECS service. \"\n        }\n      ]\n    },\n    \"cpu\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableCpu\"\n        },\n        {\n          \"description\": \" The number of CPU units used by the tasks in the Amazon ECS service. \"\n        }\n      ]\n    },\n    \"containerConfigurations\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/ContainerConfigurations\"\n        },\n        {\n          \"description\": \" The container configurations within a task of an Amazon ECS service. \"\n        }\n      ]\n    },\n    \"autoScalingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingConfiguration\"\n        },\n        {\n          \"description\": \"<p> Describes the Auto Scaling configuration methods for an Amazon ECS service. This affects the generated recommendations. For example, if Auto Scaling is configured on a service\\u2019s CPU, then Compute Optimizer doesn\\u2019t generate CPU size recommendations. </p> <p>The Auto Scaling configuration methods include:</p> <ul> <li> <p> <code>TARGET_TRACKING_SCALING_CPU</code> \\u2014 If the Amazon ECS service is configured to use target scaling on CPU, Compute Optimizer doesn't generate CPU recommendations.</p> </li> <li> <p> <code>TARGET_TRACKING_SCALING_MEMORY</code>\
  \ \\u2014 If the Amazon ECS service is configured to use target scaling on memory, Compute Optimizer doesn't generate memory recommendations.</p> </li> </ul> <p>For more information about step scaling and target scaling, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/application/userguide/application-auto-scaling-step-scaling-policies.html\\\"> Step scaling policies for Application Auto Scaling</a> and <a href=\\\"https://docs.aws.amazon.com/autoscaling/application/userguide/application-auto-scaling-target-tracking.html\\\"> Target tracking scaling policies for Application Auto Scaling</a> in the <i>Application Auto Scaling User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"taskDefinitionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskDefinitionArn\"\n        },\n        {\n          \"description\": \" The task definition ARN used by the tasks in the Amazon ECS service. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-service-configuration-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: ServiceConfiguration
---
