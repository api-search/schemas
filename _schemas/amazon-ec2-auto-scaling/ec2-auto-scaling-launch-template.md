---
description: Use this structure to specify the launch templates and instance types (overrides) for a mixed instances policy.
layout: schema
name: LaunchTemplate
properties_list:
- description: ''
  name: LaunchTemplateSpecification
  type: object
- description: ''
  name: Overrides
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-launch-template-schema.json
slug: ec2-auto-scaling-launch-template
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-launch-template-schema.json\",\n  \"title\": \"LaunchTemplate\",\n  \"description\": \"Use this structure to specify the launch templates and instance types (overrides) for a mixed instances policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LaunchTemplateSpecification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaunchTemplateSpecification\"\n        },\n        {\n          \"description\": \"The launch template.\"\n        }\n      ]\n    },\n    \"Overrides\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Overrides\"\n        },\n        {\n          \"description\": \"Any properties that you specify override the same properties in the launch template.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-launch-template-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: LaunchTemplate
---
