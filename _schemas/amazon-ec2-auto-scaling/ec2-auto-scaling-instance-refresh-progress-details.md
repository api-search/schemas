---
description: Reports progress on replacing instances in an Auto Scaling group that has a warm pool. This includes separate details for instances in the warm pool and instances in the Auto Scaling group (the live pool).
layout: schema
name: InstanceRefreshProgressDetails
properties_list:
- description: ''
  name: LivePoolProgress
  type: object
- description: ''
  name: WarmPoolProgress
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-instance-refresh-progress-details-schema.json
slug: ec2-auto-scaling-instance-refresh-progress-details
source_filename: ec2-auto-scaling-instance-refresh-progress-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-instance-refresh-progress-details-schema.json\",\n  \"title\": \"InstanceRefreshProgressDetails\",\n  \"description\": \"Reports progress on replacing instances in an Auto Scaling group that has a warm pool. This includes separate details for instances in the warm pool and instances in the Auto Scaling group (the live pool).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LivePoolProgress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceRefreshLivePoolProgress\"\n        },\n        {\n          \"description\": \"Reports progress on replacing instances that are in the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"WarmPoolProgress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceRefreshWarmPoolProgress\"\
  \n        },\n        {\n          \"description\": \"Reports progress on replacing instances that are in the warm pool.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-instance-refresh-progress-details-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: InstanceRefreshProgressDetails
---
