---
description: <p>Describes an auto scaling process that has been suspended.</p> <p>For more information, see <a href="https://docs.aws.amazon.com/autoscaling/ec2/userguide/as-suspend-resume-processes.html#process-types">Scaling processes</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p>
layout: schema
name: SuspendedProcess
properties_list:
- description: ''
  name: ProcessName
  type: object
- description: ''
  name: SuspensionReason
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-suspended-process-schema.json
slug: ec2-auto-scaling-suspended-process
source_filename: ec2-auto-scaling-suspended-process-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-suspended-process-schema.json\",\n  \"title\": \"SuspendedProcess\",\n  \"description\": \"<p>Describes an auto scaling process that has been suspended.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/as-suspend-resume-processes.html#process-types\\\">Scaling processes</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProcessName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the suspended process.\"\n        }\n      ]\n    },\n    \"SuspensionReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\
  \n        },\n        {\n          \"description\": \"The reason that the process was suspended.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-suspended-process-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: SuspendedProcess
---
