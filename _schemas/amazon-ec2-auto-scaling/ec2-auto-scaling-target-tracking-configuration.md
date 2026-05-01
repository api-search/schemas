---
description: Represents a target tracking scaling policy configuration to use with Amazon EC2 Auto Scaling.
layout: schema
name: TargetTrackingConfiguration
properties_list:
- description: ''
  name: PredefinedMetricSpecification
  type: object
- description: ''
  name: CustomizedMetricSpecification
  type: object
- description: ''
  name: TargetValue
  type: object
- description: ''
  name: DisableScaleIn
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-target-tracking-configuration-schema.json
slug: ec2-auto-scaling-target-tracking-configuration
source_filename: ec2-auto-scaling-target-tracking-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-target-tracking-configuration-schema.json\",\n  \"title\": \"TargetTrackingConfiguration\",\n  \"description\": \"Represents a target tracking scaling policy configuration to use with Amazon EC2 Auto Scaling.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PredefinedMetricSpecification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PredefinedMetricSpecification\"\n        },\n        {\n          \"description\": \"A predefined metric. You must specify either a predefined metric or a customized metric.\"\n        }\n      ]\n    },\n    \"CustomizedMetricSpecification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomizedMetricSpecification\"\n        },\n        {\n          \"description\": \"A customized\
  \ metric. You must specify either a predefined metric or a customized metric.\"\n        }\n      ]\n    },\n    \"TargetValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricScale\"\n        },\n        {\n          \"description\": \"<p>The target value for the metric.</p> <note> <p>Some metrics are based on a count instead of a percentage, such as the request count for an Application Load Balancer or the number of messages in an SQS queue. If the scaling policy specifies one of these metrics, specify the target utilization as the optimal average request or message count per instance during any one-minute interval. </p> </note>\"\n        }\n      ]\n    },\n    \"DisableScaleIn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DisableScaleIn\"\n        },\n        {\n          \"description\": \"Indicates whether scaling in by the target tracking scaling policy is disabled. If scaling in is disabled, the target tracking\
  \ scaling policy doesn't remove instances from the Auto Scaling group. Otherwise, the target tracking scaling policy can remove instances from the Auto Scaling group. The default is <code>false</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TargetValue\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-target-tracking-configuration-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: TargetTrackingConfiguration
---
