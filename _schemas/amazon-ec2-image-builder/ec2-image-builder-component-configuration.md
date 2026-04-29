---
description: Configuration details of the component.
layout: schema
name: ComponentConfiguration
properties_list:
- description: ''
  name: componentArn
  type: object
- description: ''
  name: parameters
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-component-configuration-schema.json
slug: ec2-image-builder-component-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-component-configuration-schema.json\",\n  \"title\": \"ComponentConfiguration\",\n  \"description\": \"Configuration details of the component.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"componentArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentVersionArnOrBuildVersionArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the component.\"\n        }\n      ]\n    },\n    \"parameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentParameterList\"\n        },\n        {\n          \"description\": \"A group of parameter settings that Image Builder uses to configure the component for a specific recipe.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"componentArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-component-configuration-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ComponentConfiguration
---
