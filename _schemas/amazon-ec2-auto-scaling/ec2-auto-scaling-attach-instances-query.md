---
description: AttachInstancesQuery schema from Auto Scaling
layout: schema
name: AttachInstancesQuery
properties_list:
- description: ''
  name: InstanceIds
  type: object
- description: ''
  name: AutoScalingGroupName
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-attach-instances-query-schema.json
slug: ec2-auto-scaling-attach-instances-query
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-attach-instances-query-schema.json\",\n  \"title\": \"AttachInstancesQuery\",\n  \"description\": \"AttachInstancesQuery schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceIds\"\n        },\n        {\n          \"description\": \"The IDs of the instances. You can specify up to 20 instances.\"\n        }\n      ]\n    },\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AutoScalingGroupName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-attach-instances-query-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: AttachInstancesQuery
---
