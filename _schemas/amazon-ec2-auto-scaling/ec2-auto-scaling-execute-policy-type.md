---
description: ExecutePolicyType schema from Auto Scaling
layout: schema
name: ExecutePolicyType
properties_list:
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: PolicyName
  type: object
- description: ''
  name: HonorCooldown
  type: object
- description: ''
  name: MetricValue
  type: object
- description: ''
  name: BreachThreshold
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-execute-policy-type-schema.json
slug: ec2-auto-scaling-execute-policy-type
source_filename: ec2-auto-scaling-execute-policy-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-execute-policy-type-schema.json\",\n  \"title\": \"ExecutePolicyType\",\n  \"description\": \"ExecutePolicyType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"PolicyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name or ARN of the policy.\"\n        }\n      ]\n    },\n    \"HonorCooldown\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HonorCooldown\"\n        },\n\
  \        {\n          \"description\": \"<p>Indicates whether Amazon EC2 Auto Scaling waits for the cooldown period to complete before executing the policy.</p> <p>Valid only if the policy type is <code>SimpleScaling</code>. For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/Cooldown.html\\\">Scaling cooldowns for Amazon EC2 Auto Scaling</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"MetricValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricScale\"\n        },\n        {\n          \"description\": \"<p>The metric value to compare to <code>BreachThreshold</code>. This enables you to execute a policy of type <code>StepScaling</code> and determine which step adjustment to use. For example, if the breach threshold is 50 and you want to use a step adjustment with a lower bound of 0 and an upper bound of 10, you can set the metric value to 59.</p> <p>If you specify\
  \ a metric value that doesn't correspond to a step adjustment for the policy, the call returns an error.</p> <p>Required if the policy type is <code>StepScaling</code> and not supported otherwise.</p>\"\n        }\n      ]\n    },\n    \"BreachThreshold\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricScale\"\n        },\n        {\n          \"description\": \"<p>The breach threshold for the alarm.</p> <p>Required if the policy type is <code>StepScaling</code> and not supported otherwise.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PolicyName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-execute-policy-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: ExecutePolicyType
---
