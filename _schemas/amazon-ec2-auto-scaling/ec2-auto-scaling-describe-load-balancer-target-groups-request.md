---
description: DescribeLoadBalancerTargetGroupsRequest schema from Auto Scaling
layout: schema
name: DescribeLoadBalancerTargetGroupsRequest
properties_list:
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxRecords
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-describe-load-balancer-target-groups-request-schema.json
slug: ec2-auto-scaling-describe-load-balancer-target-groups-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-load-balancer-target-groups-request-schema.json\",\n  \"title\": \"DescribeLoadBalancerTargetGroupsRequest\",\n  \"description\": \"DescribeLoadBalancerTargetGroupsRequest schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"description\": \"The token for the next set of items to return. (You received this token from a previous call.)\"\n        }\n      ]\n    },\n\
  \    \"MaxRecords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxRecords\"\n        },\n        {\n          \"description\": \"The maximum number of items to return with this call. The default value is <code>100</code> and the maximum value is <code>100</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AutoScalingGroupName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-load-balancer-target-groups-request-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: DescribeLoadBalancerTargetGroupsRequest
---
