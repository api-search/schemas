---
description: Reports progress on replacing instances that are in the Auto Scaling group.
layout: schema
name: InstanceRefreshLivePoolProgress
properties_list:
- description: ''
  name: PercentageComplete
  type: object
- description: ''
  name: InstancesToUpdate
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-instance-refresh-live-pool-progress-schema.json
slug: ec2-auto-scaling-instance-refresh-live-pool-progress
source_filename: ec2-auto-scaling-instance-refresh-live-pool-progress-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-instance-refresh-live-pool-progress-schema.json\",\n  \"title\": \"InstanceRefreshLivePoolProgress\",\n  \"description\": \"Reports progress on replacing instances that are in the Auto Scaling group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PercentageComplete\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntPercent\"\n        },\n        {\n          \"description\": \"The percentage of instances in the Auto Scaling group that have been replaced. For each instance replacement, Amazon EC2 Auto Scaling tracks the instance's health status and warm-up time. When the instance's health status changes to healthy and the specified warm-up time passes, the instance is considered updated and is added to the percentage complete.\"\n       \
  \ }\n      ]\n    },\n    \"InstancesToUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstancesToUpdate\"\n        },\n        {\n          \"description\": \"The number of instances remaining to update.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-instance-refresh-live-pool-progress-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: InstanceRefreshLivePoolProgress
---
