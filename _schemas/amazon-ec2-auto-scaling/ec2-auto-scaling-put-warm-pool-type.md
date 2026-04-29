---
description: PutWarmPoolType schema from Auto Scaling
layout: schema
name: PutWarmPoolType
properties_list:
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: MaxGroupPreparedCapacity
  type: object
- description: ''
  name: MinSize
  type: object
- description: ''
  name: PoolState
  type: object
- description: ''
  name: InstanceReusePolicy
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-put-warm-pool-type-schema.json
slug: ec2-auto-scaling-put-warm-pool-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-put-warm-pool-type-schema.json\",\n  \"title\": \"PutWarmPoolType\",\n  \"description\": \"PutWarmPoolType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"MaxGroupPreparedCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxGroupPreparedCapacity\"\n        },\n        {\n          \"description\": \"<p>Specifies the maximum number of instances that are allowed to be in the warm pool or in any state except <code>Terminated</code> for the Auto Scaling group. This is\
  \ an optional property. Specify it only if you do not want the warm pool size to be determined by the difference between the group's maximum capacity and its desired capacity. </p> <important> <p>If a value for <code>MaxGroupPreparedCapacity</code> is not specified, Amazon EC2 Auto Scaling launches and maintains the difference between the group's maximum capacity and its desired capacity. If you specify a value for <code>MaxGroupPreparedCapacity</code>, Amazon EC2 Auto Scaling uses the difference between the <code>MaxGroupPreparedCapacity</code> and the desired capacity instead. </p> <p>The size of the warm pool is dynamic. Only when <code>MaxGroupPreparedCapacity</code> and <code>MinSize</code> are set to the same value does the warm pool have an absolute size.</p> </important> <p>If the desired capacity of the Auto Scaling group is higher than the <code>MaxGroupPreparedCapacity</code>, the capacity of the warm pool is 0, unless you specify a value for <code>MinSize</code>. To remove\
  \ a value that you previously set, include the property but specify -1 for the value. </p>\"\n        }\n      ]\n    },\n    \"MinSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WarmPoolMinSize\"\n        },\n        {\n          \"description\": \"Specifies the minimum number of instances to maintain in the warm pool. This helps you to ensure that there is always a certain number of warmed instances available to handle traffic spikes. Defaults to 0 if not specified.\"\n        }\n      ]\n    },\n    \"PoolState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WarmPoolState\"\n        },\n        {\n          \"description\": \"Sets the instance state to transition to after the lifecycle actions are complete. Default is <code>Stopped</code>.\"\n        }\n      ]\n    },\n    \"InstanceReusePolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceReusePolicy\"\n        },\n     \
  \   {\n          \"description\": \"Indicates whether instances in the Auto Scaling group can be returned to the warm pool on scale in. The default is to terminate instances in the Auto Scaling group when the group scales in.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AutoScalingGroupName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-put-warm-pool-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: PutWarmPoolType
---
