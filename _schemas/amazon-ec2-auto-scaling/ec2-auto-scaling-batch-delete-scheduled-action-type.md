---
description: BatchDeleteScheduledActionType schema from Auto Scaling
layout: schema
name: BatchDeleteScheduledActionType
properties_list:
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: ScheduledActionNames
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-batch-delete-scheduled-action-type-schema.json
slug: ec2-auto-scaling-batch-delete-scheduled-action-type
source_filename: ec2-auto-scaling-batch-delete-scheduled-action-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-batch-delete-scheduled-action-type-schema.json\",\n  \"title\": \"BatchDeleteScheduledActionType\",\n  \"description\": \"BatchDeleteScheduledActionType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"ScheduledActionNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduledActionNames\"\n        },\n        {\n          \"description\": \"The names of the scheduled actions to delete. The maximum number allowed is 50. \"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"AutoScalingGroupName\",\n    \"ScheduledActionNames\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-batch-delete-scheduled-action-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: BatchDeleteScheduledActionType
---
