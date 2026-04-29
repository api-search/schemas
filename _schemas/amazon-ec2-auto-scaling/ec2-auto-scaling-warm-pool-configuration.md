---
description: Describes a warm pool configuration.
layout: schema
name: WarmPoolConfiguration
properties_list:
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
  name: Status
  type: object
- description: ''
  name: InstanceReusePolicy
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-warm-pool-configuration-schema.json
slug: ec2-auto-scaling-warm-pool-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-warm-pool-configuration-schema.json\",\n  \"title\": \"WarmPoolConfiguration\",\n  \"description\": \"Describes a warm pool configuration. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxGroupPreparedCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxGroupPreparedCapacity\"\n        },\n        {\n          \"description\": \"The maximum number of instances that are allowed to be in the warm pool or in any state except <code>Terminated</code> for the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"MinSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WarmPoolMinSize\"\n        },\n        {\n          \"description\": \"The minimum number of instances to maintain in the warm pool.\"\n\
  \        }\n      ]\n    },\n    \"PoolState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WarmPoolState\"\n        },\n        {\n          \"description\": \"The instance state to transition to after the lifecycle actions are complete.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WarmPoolStatus\"\n        },\n        {\n          \"description\": \"The status of a warm pool that is marked for deletion.\"\n        }\n      ]\n    },\n    \"InstanceReusePolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceReusePolicy\"\n        },\n        {\n          \"description\": \"The instance reuse policy.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-warm-pool-configuration-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: WarmPoolConfiguration
---
