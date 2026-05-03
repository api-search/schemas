---
description: Defines a scaling policy for automatically adjusting compute resources based on demand, applicable to cloud auto-scaling systems like KEDA, AWS Auto Scaling, Azure Autoscale, and GCP Autoscaler.
layout: schema
name: Scaling Policy
properties_list:
- description: Unique identifier name for the scaling policy.
  name: name
  type: string
- description: Namespace or resource group where the policy applies.
  name: namespace
  type: string
- description: Reference to the target resource being scaled.
  name: targetRef
  type: object
- description: Minimum number of replicas to scale down to. Set to 0 for scale-to-zero.
  name: minReplicaCount
  type: integer
- description: Maximum number of replicas to scale up to.
  name: maxReplicaCount
  type: integer
- description: Interval in seconds between polling triggers for scaling decisions.
  name: pollingInterval
  type: integer
- description: Seconds to wait after the last active trigger before scaling down.
  name: cooldownPeriod
  type: integer
- description: List of scaling triggers that drive autoscaling decisions.
  name: triggers
  type: array
- description: ''
  name: scalingBehavior
  type: object
- description: Key-value metadata labels for the scaling policy.
  name: tags
  type: object
provider_name: Scalability
provider_slug: scalability
schema_file: json-schema/scalability-scaling-policy-schema.json
slug: scalability-scaling-policy
source_filename: scalability-scaling-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/scalability/main/json-schema/scalability-scaling-policy-schema.json\",\n  \"title\": \"Scaling Policy\",\n  \"description\": \"Defines a scaling policy for automatically adjusting compute resources based on demand, applicable to cloud auto-scaling systems like KEDA, AWS Auto Scaling, Azure Autoscale, and GCP Autoscaler.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"targetRef\", \"triggers\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier name for the scaling policy.\",\n      \"minLength\": 1,\n      \"maxLength\": 253\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Namespace or resource group where the policy applies.\",\n      \"default\": \"default\"\n    },\n    \"targetRef\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Reference to the target resource being scaled.\",\n      \"required\": [\"kind\", \"name\"],\n      \"properties\": {\n        \"apiVersion\": {\n          \"type\": \"string\",\n          \"description\": \"API version of the target resource.\",\n          \"example\": \"apps/v1\"\n        },\n        \"kind\": {\n          \"type\": \"string\",\n          \"description\": \"Kind of the target resource.\",\n          \"enum\": [\"Deployment\", \"StatefulSet\", \"ReplicaSet\", \"DaemonSet\", \"Job\", \"CronJob\", \"Function\", \"ContainerApp\"]\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the target resource.\"\n        }\n      }\n    },\n    \"minReplicaCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Minimum number of replicas to scale down to. Set to 0 for scale-to-zero.\",\n      \"minimum\": 0,\n      \"default\": 0\n    },\n    \"maxReplicaCount\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Maximum number of replicas to scale up to.\",\n      \"minimum\": 1,\n      \"default\": 100\n    },\n    \"pollingInterval\": {\n      \"type\": \"integer\",\n      \"description\": \"Interval in seconds between polling triggers for scaling decisions.\",\n      \"minimum\": 1,\n      \"default\": 30\n    },\n    \"cooldownPeriod\": {\n      \"type\": \"integer\",\n      \"description\": \"Seconds to wait after the last active trigger before scaling down.\",\n      \"minimum\": 0,\n      \"default\": 300\n    },\n    \"triggers\": {\n      \"type\": \"array\",\n      \"description\": \"List of scaling triggers that drive autoscaling decisions.\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/$defs/ScalingTrigger\"\n      }\n    },\n    \"scalingBehavior\": {\n      \"$ref\": \"#/$defs/ScalingBehavior\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value metadata labels for the scaling policy.\",\n      \"additionalProperties\"\
  : {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"ScalingTrigger\": {\n      \"type\": \"object\",\n      \"description\": \"A trigger that drives autoscaling, such as CPU usage, queue depth, or custom metrics.\",\n      \"required\": [\"type\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Trigger type identifier.\",\n          \"examples\": [\"cpu\", \"memory\", \"kafka\", \"aws-sqs-queue\", \"azure-service-bus\", \"prometheus\", \"rabbitmq\", \"redis\", \"cron\"]\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Optional name for this trigger.\"\n        },\n        \"threshold\": {\n          \"type\": \"number\",\n          \"description\": \"Target metric value triggering scale-out.\",\n          \"minimum\": 0\n        },\n        \"metadata\": {\n          \"type\": \"object\",\n          \"description\": \"Trigger-specific configuration parameters.\"\
  ,\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        },\n        \"authenticationRef\": {\n          \"type\": \"object\",\n          \"description\": \"Reference to a TriggerAuthentication resource.\",\n          \"properties\": {\n            \"name\": {\n              \"type\": \"string\"\n            },\n            \"kind\": {\n              \"type\": \"string\",\n              \"enum\": [\"TriggerAuthentication\", \"ClusterTriggerAuthentication\"]\n            }\n          }\n        }\n      }\n    },\n    \"ScalingBehavior\": {\n      \"type\": \"object\",\n      \"description\": \"Controls how scaling is performed (scale-up and scale-down rates and policies).\",\n      \"properties\": {\n        \"scaleUp\": {\n          \"$ref\": \"#/$defs/ScalingRules\"\n        },\n        \"scaleDown\": {\n          \"$ref\": \"#/$defs/ScalingRules\"\n        }\n      }\n    },\n    \"ScalingRules\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Rules governing the rate and behavior of scaling in one direction.\",\n      \"properties\": {\n        \"stabilizationWindowSeconds\": {\n          \"type\": \"integer\",\n          \"description\": \"How long (in seconds) to look back at metrics before making a scaling decision.\",\n          \"minimum\": 0,\n          \"maximum\": 3600\n        },\n        \"policies\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"required\": [\"type\", \"value\", \"periodSeconds\"],\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"enum\": [\"Pods\", \"Percent\"]\n              },\n              \"value\": {\n                \"type\": \"integer\",\n                \"minimum\": 1\n              },\n              \"periodSeconds\": {\n                \"type\": \"integer\",\n                \"minimum\": 1\n              }\n            }\n          }\n        },\n       \
  \ \"selectPolicy\": {\n          \"type\": \"string\",\n          \"enum\": [\"Max\", \"Min\", \"Disabled\"],\n          \"default\": \"Max\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scalability/refs/heads/main/json-schema/scalability-scaling-policy-schema.json
tags:
- Auto Scaling
- Cloud Computing
- DevOps
- Distributed Systems
- Elasticity
- High Availability
- Infrastructure
- Load Balancing
- Performance
- Scalability
title: Scaling Policy
---
