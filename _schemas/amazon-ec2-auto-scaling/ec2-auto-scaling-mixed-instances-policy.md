---
description: <p>Use this structure to launch multiple instance types and On-Demand Instances and Spot Instances within a single Auto Scaling group.</p> <p>A mixed instances policy contains information that Amazon EC2 Auto Scaling can use to launch instances and help optimize your costs. For more information, see <a href="https://docs.aws.amazon.com/autoscaling/ec2/userguide/ec2-auto-scaling-mixed-instances-groups.html">Auto Scaling groups with multiple instance types and purchase options</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p>
layout: schema
name: MixedInstancesPolicy
properties_list:
- description: ''
  name: LaunchTemplate
  type: object
- description: ''
  name: InstancesDistribution
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-mixed-instances-policy-schema.json
slug: ec2-auto-scaling-mixed-instances-policy
source_filename: ec2-auto-scaling-mixed-instances-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-mixed-instances-policy-schema.json\",\n  \"title\": \"MixedInstancesPolicy\",\n  \"description\": \"<p>Use this structure to launch multiple instance types and On-Demand Instances and Spot Instances within a single Auto Scaling group.</p> <p>A mixed instances policy contains information that Amazon EC2 Auto Scaling can use to launch instances and help optimize your costs. For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/ec2-auto-scaling-mixed-instances-groups.html\\\">Auto Scaling groups with multiple instance types and purchase options</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LaunchTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaunchTemplate\"\
  \n        },\n        {\n          \"description\": \"One or more launch templates and the instance types (overrides) that are used to launch EC2 instances to fulfill On-Demand and Spot capacities.\"\n        }\n      ]\n    },\n    \"InstancesDistribution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstancesDistribution\"\n        },\n        {\n          \"description\": \"The instances distribution.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-mixed-instances-policy-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: MixedInstancesPolicy
---
