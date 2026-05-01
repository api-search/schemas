---
description: StartInstanceRefreshType schema from Auto Scaling
layout: schema
name: StartInstanceRefreshType
properties_list:
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: Strategy
  type: object
- description: ''
  name: DesiredConfiguration
  type: object
- description: ''
  name: Preferences
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-start-instance-refresh-type-schema.json
slug: ec2-auto-scaling-start-instance-refresh-type
source_filename: ec2-auto-scaling-start-instance-refresh-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-start-instance-refresh-type-schema.json\",\n  \"title\": \"StartInstanceRefreshType\",\n  \"description\": \"StartInstanceRefreshType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"Strategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RefreshStrategy\"\n        },\n        {\n          \"description\": \"The strategy to use for the instance refresh. The only valid value is <code>Rolling</code>.\"\n        }\n      ]\n    },\n    \"DesiredConfiguration\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DesiredConfiguration\"\n        },\n        {\n          \"description\": \"<p>The desired configuration. For example, the desired configuration can specify a new launch template or a new version of the current launch template.</p> <p>Once the instance refresh succeeds, Amazon EC2 Auto Scaling updates the settings of the Auto Scaling group to reflect the new desired configuration. </p> <note> <p>When you specify a new launch template or a new version of the current launch template for your desired configuration, consider enabling the <code>SkipMatching</code> property in preferences. If it's enabled, Amazon EC2 Auto Scaling skips replacing instances that already use the specified launch template and instance types. This can help you reduce the number of replacements that are required to apply updates. </p> </note>\"\n        }\n      ]\n    },\n    \"Preferences\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/RefreshPreferences\"\n        },\n        {\n          \"description\": \"<p>Sets your preferences for the instance refresh so that it performs as expected when you start it. Includes the instance warmup time, the minimum healthy percentage, and the behaviors that you want Amazon EC2 Auto Scaling to use if instances that are in <code>Standby</code> state or protected from scale in are found. You can also choose to enable additional features, such as the following:</p> <ul> <li> <p>Auto rollback</p> </li> <li> <p>Checkpoints</p> </li> <li> <p>Skip matching</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AutoScalingGroupName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-start-instance-refresh-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: StartInstanceRefreshType
---
