---
description: Describes a block device mapping.
layout: schema
name: BlockDeviceMapping
properties_list:
- description: ''
  name: VirtualName
  type: object
- description: ''
  name: DeviceName
  type: object
- description: ''
  name: Ebs
  type: object
- description: ''
  name: NoDevice
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-block-device-mapping-schema.json
slug: ec2-auto-scaling-block-device-mapping
source_filename: ec2-auto-scaling-block-device-mapping-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-block-device-mapping-schema.json\",\n  \"title\": \"BlockDeviceMapping\",\n  \"description\": \"Describes a block device mapping.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VirtualName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the instance store volume (virtual device) to attach to an instance at launch. The name must be in the form ephemeral<i>X</i> where <i>X</i> is a number starting from zero (0), for example, <code>ephemeral0</code>.\"\n        }\n      ]\n    },\n    \"DeviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"<p>The\
  \ device name assigned to the volume (for example, <code>/dev/sdh</code> or <code>xvdh</code>). For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/device_naming.html\\\">Device naming on Linux instances</a> in the <i>Amazon EC2 User Guide for Linux Instances</i>.</p> <note> <p>To define a block device mapping, set the device name and exactly one of the following properties: <code>Ebs</code>, <code>NoDevice</code>, or <code>VirtualName</code>.</p> </note>\"\n        }\n      ]\n    },\n    \"Ebs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ebs\"\n        },\n        {\n          \"description\": \"Information to attach an EBS volume to an instance at launch.\"\n        }\n      ]\n    },\n    \"NoDevice\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NoDevice\"\n        },\n        {\n          \"description\": \"<p>Setting this value to <code>true</code> prevents a volume that is included\
  \ in the block device mapping of the AMI from being mapped to the specified device name at launch.</p> <p>If <code>NoDevice</code> is <code>true</code> for the root device, instances might fail the EC2 health check. In that case, Amazon EC2 Auto Scaling launches replacement instances.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DeviceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-block-device-mapping-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: BlockDeviceMapping
---
