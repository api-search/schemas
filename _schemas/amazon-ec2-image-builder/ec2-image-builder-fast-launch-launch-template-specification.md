---
description: <p>Identifies the launch template that the associated Windows AMI uses for launching an instance when faster launching is enabled.</p> <note> <p>You can specify either the <code>launchTemplateName</code> or the <code>launchTemplateId</code>, but not both.</p> </note>
layout: schema
name: FastLaunchLaunchTemplateSpecification
properties_list:
- description: ''
  name: launchTemplateId
  type: object
- description: ''
  name: launchTemplateName
  type: object
- description: ''
  name: launchTemplateVersion
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-fast-launch-launch-template-specification-schema.json
slug: ec2-image-builder-fast-launch-launch-template-specification
source_filename: ec2-image-builder-fast-launch-launch-template-specification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-fast-launch-launch-template-specification-schema.json\",\n  \"title\": \"FastLaunchLaunchTemplateSpecification\",\n  \"description\": \"<p>Identifies the launch template that the associated Windows AMI uses for launching an instance when faster launching is enabled.</p> <note> <p>You can specify either the <code>launchTemplateName</code> or the <code>launchTemplateId</code>, but not both.</p> </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"launchTemplateId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaunchTemplateId\"\n        },\n        {\n          \"description\": \"The ID of the launch template to use for faster launching for a Windows AMI.\"\n        }\n      ]\n    },\n    \"launchTemplateName\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of the launch template to use for faster launching for a Windows AMI.\"\n        }\n      ]\n    },\n    \"launchTemplateVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The version of the launch template to use for faster launching for a Windows AMI.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-fast-launch-launch-template-specification-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: FastLaunchLaunchTemplateSpecification
---
