---
description: Represents a metric pair for a predictive scaling policy.
layout: schema
name: PredictiveScalingPredefinedMetricPair
properties_list:
- description: ''
  name: PredefinedMetricType
  type: object
- description: ''
  name: ResourceLabel
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-predictive-scaling-predefined-metric-pair-schema.json
slug: ec2-auto-scaling-predictive-scaling-predefined-metric-pair
source_filename: ec2-auto-scaling-predictive-scaling-predefined-metric-pair-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-predictive-scaling-predefined-metric-pair-schema.json\",\n  \"title\": \"PredictiveScalingPredefinedMetricPair\",\n  \"description\": \"Represents a metric pair for a predictive scaling policy. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PredefinedMetricType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PredefinedMetricPairType\"\n        },\n        {\n          \"description\": \"Indicates which metrics to use. There are two different types of metrics for each metric type: one is a load metric and one is a scaling metric. For example, if the metric type is <code>ASGCPUUtilization</code>, the Auto Scaling group's total CPU metric is used as the load metric, and the average CPU metric is used for the scaling metric.\"\n        }\n\
  \      ]\n    },\n    \"ResourceLabel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen1023\"\n        },\n        {\n          \"description\": \"<p>A label that uniquely identifies a specific Application Load Balancer target group from which to determine the total and average request count served by your Auto Scaling group. You can't specify a resource label unless the target group is attached to the Auto Scaling group.</p> <p>You create the resource label by appending the final portion of the load balancer ARN and the final portion of the target group ARN into a single value, separated by a forward slash (/). The format of the resource label is:</p> <p> <code>app/my-alb/778d41231b141a0f/targetgroup/my-alb-target-group/943f017f100becff</code>.</p> <p>Where:</p> <ul> <li> <p>app/&lt;load-balancer-name&gt;/&lt;load-balancer-id&gt; is the final portion of the load balancer ARN</p> </li> <li> <p>targetgroup/&lt;target-group-name&gt;/&lt;target-group-id&gt;\
  \ is the final portion of the target group ARN.</p> </li> </ul> <p>To find the ARN for an Application Load Balancer, use the <a href=\\\"https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_DescribeLoadBalancers.html\\\">DescribeLoadBalancers</a> API operation. To find the ARN for the target group, use the <a href=\\\"https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_DescribeTargetGroups.html\\\">DescribeTargetGroups</a> API operation.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PredefinedMetricType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-predictive-scaling-predefined-metric-pair-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: PredictiveScalingPredefinedMetricPair
---
