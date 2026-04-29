---
description: DescribeLoadBalancersResponse schema from Auto Scaling
layout: schema
name: DescribeLoadBalancersResponse
properties_list:
- description: ''
  name: LoadBalancers
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-describe-load-balancers-response-schema.json
slug: ec2-auto-scaling-describe-load-balancers-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-load-balancers-response-schema.json\",\n  \"title\": \"DescribeLoadBalancersResponse\",\n  \"description\": \"DescribeLoadBalancersResponse schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LoadBalancers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoadBalancerStates\"\n        },\n        {\n          \"description\": \"The load balancers.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"description\": \"A string that indicates that the response contains more items than can be returned in a single response. To receive additional items, specify this string for the <code>NextToken</code>\
  \ value when requesting the next set of items. This value is null when there are no more items to return.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"LoadBalancers\": [\n      {\n        \"LoadBalancerName\": \"my-load-balancer\",\n        \"State\": \"Added\"\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-load-balancers-response-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: DescribeLoadBalancersResponse
---
