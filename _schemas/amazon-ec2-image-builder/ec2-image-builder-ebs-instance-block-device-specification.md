---
description: Amazon EBS-specific block device mapping specifications.
layout: schema
name: EbsInstanceBlockDeviceSpecification
properties_list:
- description: ''
  name: encrypted
  type: object
- description: ''
  name: deleteOnTermination
  type: object
- description: ''
  name: iops
  type: object
- description: ''
  name: kmsKeyId
  type: object
- description: ''
  name: snapshotId
  type: object
- description: ''
  name: volumeSize
  type: object
- description: ''
  name: volumeType
  type: object
- description: ''
  name: throughput
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-ebs-instance-block-device-specification-schema.json
slug: ec2-image-builder-ebs-instance-block-device-specification
source_filename: ec2-image-builder-ebs-instance-block-device-specification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-ebs-instance-block-device-specification-schema.json\",\n  \"title\": \"EbsInstanceBlockDeviceSpecification\",\n  \"description\": \"Amazon EBS-specific block device mapping specifications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"encrypted\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"Use to configure device encryption.\"\n        }\n      ]\n    },\n    \"deleteOnTermination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"Use to configure delete on termination of the associated device.\"\n        }\n      ]\n    },\n    \"iops\": {\n      \"allOf\": [\n  \
  \      {\n          \"$ref\": \"#/components/schemas/EbsIopsInteger\"\n        },\n        {\n          \"description\": \"Use to configure device IOPS.\"\n        }\n      ]\n    },\n    \"kmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"Use to configure the KMS key to use when encrypting the device.\"\n        }\n      ]\n    },\n    \"snapshotId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The snapshot that defines the device contents.\"\n        }\n      ]\n    },\n    \"volumeSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EbsVolumeSizeInteger\"\n        },\n        {\n          \"description\": \"Use to override the device's volume size.\"\n        }\n      ]\n    },\n    \"volumeType\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/EbsVolumeType\"\n        },\n        {\n          \"description\": \"Use to override the device's volume type.\"\n        }\n      ]\n    },\n    \"throughput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EbsVolumeThroughput\"\n        },\n        {\n          \"description\": \" <b>For GP3 volumes only</b> \\u2013 The throughput in MiB/s that the volume supports.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-ebs-instance-block-device-specification-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: EbsInstanceBlockDeviceSpecification
---
