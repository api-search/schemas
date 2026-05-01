---
description: The resources produced by this image.
layout: schema
name: OutputResources
properties_list:
- description: ''
  name: amis
  type: object
- description: ''
  name: containers
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-output-resources-schema.json
slug: ec2-image-builder-output-resources
source_filename: ec2-image-builder-output-resources-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-output-resources-schema.json\",\n  \"title\": \"OutputResources\",\n  \"description\": \"The resources produced by this image.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amis\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmiList\"\n        },\n        {\n          \"description\": \"The Amazon EC2 AMIs created by this image.\"\n        }\n      ]\n    },\n    \"containers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerList\"\n        },\n        {\n          \"description\": \"Container images that the pipeline has generated and stored in the output repository.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-output-resources-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: OutputResources
---
