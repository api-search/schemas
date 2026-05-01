---
description: Defines a custom base AMI and block device mapping configurations of an instance used for building and testing container images.
layout: schema
name: InstanceConfiguration
properties_list:
- description: ''
  name: image
  type: object
- description: ''
  name: blockDeviceMappings
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-instance-configuration-schema.json
slug: ec2-image-builder-instance-configuration
source_filename: ec2-image-builder-instance-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-instance-configuration-schema.json\",\n  \"title\": \"InstanceConfiguration\",\n  \"description\": \"Defines a custom base AMI and block device mapping configurations of an instance used for building and testing container images.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"image\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The AMI ID to use as the base image for a container build and test instance. If not specified, Image Builder will use the appropriate ECS-optimized AMI as a base image.\"\n        }\n      ]\n    },\n    \"blockDeviceMappings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceBlockDeviceMappings\"\n      \
  \  },\n        {\n          \"description\": \"Defines the block devices to attach for building an instance from this Image Builder AMI.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-instance-configuration-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: InstanceConfiguration
---
