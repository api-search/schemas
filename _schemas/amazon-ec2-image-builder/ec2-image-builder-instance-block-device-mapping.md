---
description: Defines block device mappings for the instance used to configure your image.
layout: schema
name: InstanceBlockDeviceMapping
properties_list:
- description: ''
  name: deviceName
  type: object
- description: ''
  name: ebs
  type: object
- description: ''
  name: virtualName
  type: object
- description: ''
  name: noDevice
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-instance-block-device-mapping-schema.json
slug: ec2-image-builder-instance-block-device-mapping
source_filename: ec2-image-builder-instance-block-device-mapping-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-instance-block-device-mapping-schema.json\",\n  \"title\": \"InstanceBlockDeviceMapping\",\n  \"description\": \"Defines block device mappings for the instance used to configure your image.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The device to which these mappings apply.\"\n        }\n      ]\n    },\n    \"ebs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EbsInstanceBlockDeviceSpecification\"\n        },\n        {\n          \"description\": \"Use to manage Amazon EBS-specific configuration for this mapping.\"\n        }\n      ]\n    },\n    \"virtualName\": {\n   \
  \   \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"Use to manage instance ephemeral devices.\"\n        }\n      ]\n    },\n    \"noDevice\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmptyString\"\n        },\n        {\n          \"description\": \"Use to remove a mapping from the base image.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-instance-block-device-mapping-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: InstanceBlockDeviceMapping
---
