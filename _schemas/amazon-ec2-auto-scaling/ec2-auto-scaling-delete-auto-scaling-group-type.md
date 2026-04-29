---
description: DeleteAutoScalingGroupType schema from Auto Scaling
layout: schema
name: DeleteAutoScalingGroupType
properties_list:
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: ForceDelete
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-delete-auto-scaling-group-type-schema.json
slug: ec2-auto-scaling-delete-auto-scaling-group-type
source_filename: ec2-auto-scaling-delete-auto-scaling-group-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-delete-auto-scaling-group-type-schema.json\",\n  \"title\": \"DeleteAutoScalingGroupType\",\n  \"description\": \"DeleteAutoScalingGroupType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"ForceDelete\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ForceDelete\"\n        },\n        {\n          \"description\": \"Specifies that the group is to be deleted along with all instances associated with the group, without waiting for all instances to be terminated. This action also\
  \ deletes any outstanding lifecycle actions associated with the group.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AutoScalingGroupName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-delete-auto-scaling-group-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: DeleteAutoScalingGroupType
---
