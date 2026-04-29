---
description: A JSON-formatted object that contains the IDs for an Amazon Machine Image (AMI), including the Amazon EC2-compatible AMI ID and the Snow device AMI ID. Each AMI has these two IDs to simplify identifying the AMI in both the Amazon Web Services Cloud and on the device.
layout: schema
name: Ec2AmiResource
properties_list:
- description: ''
  name: AmiId
  type: object
- description: ''
  name: SnowballAmiId
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-ec2-ami-resource-schema.json
slug: amazon-snow-family-ec2-ami-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-ec2-ami-resource-schema.json\",\n  \"title\": \"Ec2AmiResource\",\n  \"description\": \"A JSON-formatted object that contains the IDs for an Amazon Machine Image (AMI), including the Amazon EC2-compatible AMI ID and the Snow device AMI ID. Each AMI has these two IDs to simplify identifying the AMI in both the Amazon Web Services Cloud and on the device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AmiId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmiId\"\n        },\n        {\n          \"description\": \"The ID of the AMI in Amazon EC2.\"\n        }\n      ]\n    },\n    \"SnowballAmiId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ID\
  \ of the AMI on the Snow device.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AmiId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-ec2-ami-resource-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: Ec2AmiResource
---
