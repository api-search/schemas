---
description: Contains settings for the Systems Manager agent on your build instance.
layout: schema
name: SystemsManagerAgent
properties_list:
- description: ''
  name: uninstallAfterBuild
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-systems-manager-agent-schema.json
slug: ec2-image-builder-systems-manager-agent
source_filename: ec2-image-builder-systems-manager-agent-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-systems-manager-agent-schema.json\",\n  \"title\": \"SystemsManagerAgent\",\n  \"description\": \"Contains settings for the Systems Manager agent on your build instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uninstallAfterBuild\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"Controls whether the Systems Manager agent is removed from your final build image, prior to creating the new AMI. If this is set to true, then the agent is removed from the final image. If it's set to false, then the agent is left in, so that it is included in the new AMI. The default value is false.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-systems-manager-agent-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: SystemsManagerAgent
---
