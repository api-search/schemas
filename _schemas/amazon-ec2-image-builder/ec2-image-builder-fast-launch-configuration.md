---
description: Define and configure faster launching for output Windows AMIs.
layout: schema
name: FastLaunchConfiguration
properties_list:
- description: ''
  name: enabled
  type: object
- description: ''
  name: snapshotConfiguration
  type: object
- description: ''
  name: maxParallelLaunches
  type: object
- description: ''
  name: launchTemplate
  type: object
- description: ''
  name: accountId
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-fast-launch-configuration-schema.json
slug: ec2-image-builder-fast-launch-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-fast-launch-configuration-schema.json\",\n  \"title\": \"FastLaunchConfiguration\",\n  \"description\": \"Define and configure faster launching for output Windows AMIs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A Boolean that represents the current state of faster launching for the Windows AMI. Set to <code>true</code> to start using Windows faster launching, or <code>false</code> to stop using it.\"\n        }\n      ]\n    },\n    \"snapshotConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FastLaunchSnapshotConfiguration\"\n        },\n        {\n          \"description\"\
  : \"Configuration settings for managing the number of snapshots that are created from pre-provisioned instances for the Windows AMI when faster launching is enabled.\"\n        }\n      ]\n    },\n    \"maxParallelLaunches\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxParallelLaunches\"\n        },\n        {\n          \"description\": \"The maximum number of parallel instances that are launched for creating resources.\"\n        }\n      ]\n    },\n    \"launchTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FastLaunchLaunchTemplateSpecification\"\n        },\n        {\n          \"description\": \"The launch template that the fast-launch enabled Windows AMI uses when it launches Windows instances to create pre-provisioned snapshots.\"\n        }\n      ]\n    },\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"\
  description\": \"The owner account ID for the fast-launch enabled Windows AMI.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"enabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-fast-launch-configuration-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: FastLaunchConfiguration
---
