---
description: Identifying information for a traffic source.
layout: schema
name: TrafficSourceIdentifier
properties_list:
- description: ''
  name: Identifier
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-traffic-source-identifier-schema.json
slug: ec2-auto-scaling-traffic-source-identifier
source_filename: ec2-auto-scaling-traffic-source-identifier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-traffic-source-identifier-schema.json\",\n  \"title\": \"TrafficSourceIdentifier\",\n  \"description\": \"Identifying information for a traffic source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Identifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen511\"\n        },\n        {\n          \"description\": \"<p>Identifies the traffic source.</p> <p>For Application Load Balancers, Gateway Load Balancers, Network Load Balancers, and VPC Lattice, this will be the Amazon Resource Name (ARN) for a target group in this account and Region. For Classic Load Balancers, this will be the name of the Classic Load Balancer in this account and Region.</p> <p>For example: </p> <ul> <li> <p>Application Load Balancer ARN: <code>arn:aws:elasticloadbalancing:us-west-2:123456789012:targetgroup/my-targets/1234567890123456</code>\
  \ </p> </li> <li> <p>Classic Load Balancer name: <code>my-classic-load-balancer</code> </p> </li> <li> <p>VPC Lattice ARN: <code>arn:aws:vpc-lattice:us-west-2:123456789012:targetgroup/tg-1234567890123456</code> </p> </li> </ul> <p>To get the ARN of a target group for a Application Load Balancer, Gateway Load Balancer, or Network Load Balancer, or the name of a Classic Load Balancer, use the Elastic Load Balancing <a href=\\\"https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_DescribeTargetGroups.html\\\">DescribeTargetGroups</a> and <a href=\\\"https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_DescribeLoadBalancers.html\\\">DescribeLoadBalancers</a> API operations.</p> <p>To get the ARN of a target group for VPC Lattice, use the VPC Lattice <a href=\\\"https://docs.aws.amazon.com/vpc-lattice/latest/APIReference/API_GetTargetGroup.html\\\">GetTargetGroup</a> API operation.</p>\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen511\"\n        },\n        {\n          \"description\": \"<p>Provides additional context for the value of <code>Identifier</code>.</p> <p>The following lists the valid values:</p> <ul> <li> <p> <code>elb</code> if <code>Identifier</code> is the name of a Classic Load Balancer.</p> </li> <li> <p> <code>elbv2</code> if <code>Identifier</code> is the ARN of an Application Load Balancer, Gateway Load Balancer, or Network Load Balancer target group.</p> </li> <li> <p> <code>vpc-lattice</code> if <code>Identifier</code> is the ARN of a VPC Lattice target group.</p> </li> </ul> <p>Required if the identifier is the name of a Classic Load Balancer.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Identifier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-traffic-source-identifier-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: TrafficSourceIdentifier
---
