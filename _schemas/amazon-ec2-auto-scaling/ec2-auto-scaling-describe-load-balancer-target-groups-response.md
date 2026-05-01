---
description: DescribeLoadBalancerTargetGroupsResponse schema from Auto Scaling
layout: schema
name: DescribeLoadBalancerTargetGroupsResponse
properties_list:
- description: ''
  name: LoadBalancerTargetGroups
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-describe-load-balancer-target-groups-response-schema.json
slug: ec2-auto-scaling-describe-load-balancer-target-groups-response
source_filename: ec2-auto-scaling-describe-load-balancer-target-groups-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-load-balancer-target-groups-response-schema.json\",\n  \"title\": \"DescribeLoadBalancerTargetGroupsResponse\",\n  \"description\": \"DescribeLoadBalancerTargetGroupsResponse schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LoadBalancerTargetGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoadBalancerTargetGroupStates\"\n        },\n        {\n          \"description\": \"Information about the target groups.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"description\": \"A string that indicates that the response contains more items than can be returned in a single response.\
  \ To receive additional items, specify this string for the <code>NextToken</code> value when requesting the next set of items. This value is null when there are no more items to return.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"LoadBalancerTargetGroups\": [\n      {\n        \"LoadBalancerTargetGroupARN\": \"arn:aws:elasticloadbalancing:us-west-2:123456789012:targetgroup/my-targets/73e2d6bc24d8a067\",\n        \"State\": \"Added\"\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-load-balancer-target-groups-response-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: DescribeLoadBalancerTargetGroupsResponse
---
