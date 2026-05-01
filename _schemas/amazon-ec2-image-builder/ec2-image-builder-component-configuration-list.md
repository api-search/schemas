---
description: ComponentConfigurationList schema from EC2 Image Builder
layout: schema
name: ComponentConfigurationList
properties_list: []
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-component-configuration-list-schema.json
slug: ec2-image-builder-component-configuration-list
source_filename: ec2-image-builder-component-configuration-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-component-configuration-list-schema.json\",\n  \"title\": \"ComponentConfigurationList\",\n  \"description\": \"ComponentConfigurationList schema from EC2 Image Builder\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/ComponentConfiguration\"\n  },\n  \"minItems\": 1\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-component-configuration-list-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ComponentConfigurationList
---
