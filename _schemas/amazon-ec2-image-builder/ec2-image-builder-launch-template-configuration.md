---
description: Identifies an Amazon EC2 launch template to use for a specific account.
layout: schema
name: LaunchTemplateConfiguration
properties_list:
- description: ''
  name: launchTemplateId
  type: object
- description: ''
  name: accountId
  type: object
- description: ''
  name: setDefaultVersion
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-launch-template-configuration-schema.json
slug: ec2-image-builder-launch-template-configuration
source_filename: ec2-image-builder-launch-template-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-launch-template-configuration-schema.json\",\n  \"title\": \"LaunchTemplateConfiguration\",\n  \"description\": \"Identifies an Amazon EC2 launch template to use for a specific account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"launchTemplateId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaunchTemplateId\"\n        },\n        {\n          \"description\": \"Identifies the Amazon EC2 launch template to use.\"\n        }\n      ]\n    },\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The account ID that this configuration applies to.\"\n        }\n      ]\n    },\n    \"setDefaultVersion\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Set the specified Amazon EC2 launch template as the default launch template for the specified account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"launchTemplateId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-launch-template-configuration-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: LaunchTemplateConfiguration
---
