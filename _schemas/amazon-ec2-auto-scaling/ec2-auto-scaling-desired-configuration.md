---
description: <p>Describes the desired configuration for an instance refresh. </p> <p>If you specify a desired configuration, you must specify either a <code>LaunchTemplate</code> or a <code>MixedInstancesPolicy</code>. </p>
layout: schema
name: DesiredConfiguration
properties_list:
- description: ''
  name: LaunchTemplate
  type: object
- description: ''
  name: MixedInstancesPolicy
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-desired-configuration-schema.json
slug: ec2-auto-scaling-desired-configuration
source_filename: ec2-auto-scaling-desired-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-desired-configuration-schema.json\",\n  \"title\": \"DesiredConfiguration\",\n  \"description\": \"<p>Describes the desired configuration for an instance refresh. </p> <p>If you specify a desired configuration, you must specify either a <code>LaunchTemplate</code> or a <code>MixedInstancesPolicy</code>. </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LaunchTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaunchTemplateSpecification\"\n        },\n        {\n          \"description\": \"Describes the launch template and the version of the launch template that Amazon EC2 Auto Scaling uses to launch Amazon EC2 instances. For more information about launch templates, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/LaunchTemplates.html\\\
  \">Launch templates</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.\"\n        }\n      ]\n    },\n    \"MixedInstancesPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MixedInstancesPolicy\"\n        },\n        {\n          \"description\": \"<p>Use this structure to launch multiple instance types and On-Demand Instances and Spot Instances within a single Auto Scaling group.</p> <p>A mixed instances policy contains information that Amazon EC2 Auto Scaling can use to launch instances and help optimize your costs. For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/ec2-auto-scaling-mixed-instances-groups.html\\\">Auto Scaling groups with multiple instance types and purchase options</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-desired-configuration-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: DesiredConfiguration
---
