---
description: DescribeTerminationPolicyTypesAnswer schema from Auto Scaling
layout: schema
name: DescribeTerminationPolicyTypesAnswer
properties_list:
- description: ''
  name: TerminationPolicyTypes
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-describe-termination-policy-types-answer-schema.json
slug: ec2-auto-scaling-describe-termination-policy-types-answer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-termination-policy-types-answer-schema.json\",\n  \"title\": \"DescribeTerminationPolicyTypesAnswer\",\n  \"description\": \"DescribeTerminationPolicyTypesAnswer schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TerminationPolicyTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TerminationPolicies\"\n        },\n        {\n          \"description\": \"The termination policies supported by Amazon EC2 Auto Scaling: <code>OldestInstance</code>, <code>OldestLaunchConfiguration</code>, <code>NewestInstance</code>, <code>ClosestToNextInstanceHour</code>, <code>Default</code>, <code>OldestLaunchTemplate</code>, and <code>AllocationStrategy</code>.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"TerminationPolicyTypes\"\
  : [\n      \"ClosestToNextInstanceHour\",\n      \"Default\",\n      \"NewestInstance\",\n      \"OldestInstance\",\n      \"OldestLaunchConfiguration\"\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-termination-policy-types-answer-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: DescribeTerminationPolicyTypesAnswer
---
