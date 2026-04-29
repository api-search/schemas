---
description: <p>Describes an instance reuse policy for a warm pool. </p> <p>For more information, see <a href="https://docs.aws.amazon.com/autoscaling/ec2/userguide/ec2-auto-scaling-warm-pools.html">Warm pools for Amazon EC2 Auto Scaling</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p>
layout: schema
name: InstanceReusePolicy
properties_list:
- description: ''
  name: ReuseOnScaleIn
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-instance-reuse-policy-schema.json
slug: ec2-auto-scaling-instance-reuse-policy
source_filename: ec2-auto-scaling-instance-reuse-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-instance-reuse-policy-schema.json\",\n  \"title\": \"InstanceReusePolicy\",\n  \"description\": \"<p>Describes an instance reuse policy for a warm pool. </p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/ec2-auto-scaling-warm-pools.html\\\">Warm pools for Amazon EC2 Auto Scaling</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReuseOnScaleIn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReuseOnScaleIn\"\n        },\n        {\n          \"description\": \"Specifies whether instances in the Auto Scaling group can be returned to the warm pool on scale in. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-instance-reuse-policy-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: InstanceReusePolicy
---
