---
description: CompleteLifecycleActionType schema from Auto Scaling
layout: schema
name: CompleteLifecycleActionType
properties_list:
- description: ''
  name: LifecycleHookName
  type: object
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: LifecycleActionToken
  type: object
- description: ''
  name: LifecycleActionResult
  type: object
- description: ''
  name: InstanceId
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-complete-lifecycle-action-type-schema.json
slug: ec2-auto-scaling-complete-lifecycle-action-type
source_filename: ec2-auto-scaling-complete-lifecycle-action-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-complete-lifecycle-action-type-schema.json\",\n  \"title\": \"CompleteLifecycleActionType\",\n  \"description\": \"CompleteLifecycleActionType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LifecycleHookName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AsciiStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the lifecycle hook.\"\n        }\n      ]\n    },\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"LifecycleActionToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/LifecycleActionToken\"\n        },\n        {\n          \"description\": \"A universally unique identifier (UUID) that identifies a specific lifecycle action associated with an instance. Amazon EC2 Auto Scaling sends this token to the notification target you specified when you created the lifecycle hook.\"\n        }\n      ]\n    },\n    \"LifecycleActionResult\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LifecycleActionResult\"\n        },\n        {\n          \"description\": \"The action for the group to take. You can specify either <code>CONTINUE</code> or <code>ABANDON</code>.\"\n        }\n      ]\n    },\n    \"InstanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen19\"\n        },\n        {\n          \"description\": \"The ID of the instance.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LifecycleHookName\",\n    \"AutoScalingGroupName\",\n    \"LifecycleActionResult\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-complete-lifecycle-action-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: CompleteLifecycleActionType
---
