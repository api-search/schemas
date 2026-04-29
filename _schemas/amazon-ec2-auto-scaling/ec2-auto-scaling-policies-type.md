---
description: PoliciesType schema from Auto Scaling
layout: schema
name: PoliciesType
properties_list:
- description: ''
  name: ScalingPolicies
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-policies-type-schema.json
slug: ec2-auto-scaling-policies-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-policies-type-schema.json\",\n  \"title\": \"PoliciesType\",\n  \"description\": \"PoliciesType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ScalingPolicies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScalingPolicies\"\n        },\n        {\n          \"description\": \"The scaling policies.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"description\": \"A string that indicates that the response contains more items than can be returned in a single response. To receive additional items, specify this string for the <code>NextToken</code> value when requesting the next set of items.\
  \ This value is null when there are no more items to return.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"ScalingPolicies\": [\n      {\n        \"AdjustmentType\": \"ChangeInCapacity\",\n        \"Alarms\": [],\n        \"AutoScalingGroupName\": \"my-auto-scaling-group\",\n        \"PolicyARN\": \"arn:aws:autoscaling:us-west-2:123456789012:scalingPolicy:2233f3d7-6290-403b-b632-93c553560106:autoScalingGroupName/my-auto-scaling-group:policyName/ScaleIn\",\n        \"PolicyName\": \"ScaleIn\",\n        \"ScalingAdjustment\": -1\n      },\n      {\n        \"AdjustmentType\": \"PercentChangeInCapacity\",\n        \"Alarms\": [],\n        \"AutoScalingGroupName\": \"my-auto-scaling-group\",\n        \"Cooldown\": 60,\n        \"MinAdjustmentStep\": 2,\n        \"PolicyARN\": \"arn:aws:autoscaling:us-west-2:123456789012:scalingPolicy:2b435159-cf77-4e89-8c0e-d63b497baad7:autoScalingGroupName/my-auto-scaling-group:policyName/ScalePercentChange\",\n        \"PolicyName\": \"ScalePercentChange\"\
  ,\n        \"ScalingAdjustment\": 25\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-policies-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: PoliciesType
---
