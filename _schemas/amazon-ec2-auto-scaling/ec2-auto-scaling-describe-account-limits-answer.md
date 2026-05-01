---
description: DescribeAccountLimitsAnswer schema from Auto Scaling
layout: schema
name: DescribeAccountLimitsAnswer
properties_list:
- description: ''
  name: MaxNumberOfAutoScalingGroups
  type: object
- description: ''
  name: MaxNumberOfLaunchConfigurations
  type: object
- description: ''
  name: NumberOfAutoScalingGroups
  type: object
- description: ''
  name: NumberOfLaunchConfigurations
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-describe-account-limits-answer-schema.json
slug: ec2-auto-scaling-describe-account-limits-answer
source_filename: ec2-auto-scaling-describe-account-limits-answer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-account-limits-answer-schema.json\",\n  \"title\": \"DescribeAccountLimitsAnswer\",\n  \"description\": \"DescribeAccountLimitsAnswer schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxNumberOfAutoScalingGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxNumberOfAutoScalingGroups\"\n        },\n        {\n          \"description\": \"The maximum number of groups allowed for your account. The default is 200 groups per Region.\"\n        }\n      ]\n    },\n    \"MaxNumberOfLaunchConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxNumberOfLaunchConfigurations\"\n        },\n        {\n          \"description\": \"The maximum number of launch configurations\
  \ allowed for your account. The default is 200 launch configurations per Region.\"\n        }\n      ]\n    },\n    \"NumberOfAutoScalingGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NumberOfAutoScalingGroups\"\n        },\n        {\n          \"description\": \"The current number of groups for your account.\"\n        }\n      ]\n    },\n    \"NumberOfLaunchConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NumberOfLaunchConfigurations\"\n        },\n        {\n          \"description\": \"The current number of launch configurations for your account.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"MaxNumberOfAutoScalingGroups\": 20,\n    \"MaxNumberOfLaunchConfigurations\": 100,\n    \"NumberOfAutoScalingGroups\": 3,\n    \"NumberOfLaunchConfigurations\": 5\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-account-limits-answer-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: DescribeAccountLimitsAnswer
---
