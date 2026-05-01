---
description: Configuration settings for creating and managing pre-provisioned snapshots for a fast-launch enabled Windows AMI.
layout: schema
name: FastLaunchSnapshotConfiguration
properties_list:
- description: ''
  name: targetResourceCount
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-fast-launch-snapshot-configuration-schema.json
slug: ec2-image-builder-fast-launch-snapshot-configuration
source_filename: ec2-image-builder-fast-launch-snapshot-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-fast-launch-snapshot-configuration-schema.json\",\n  \"title\": \"FastLaunchSnapshotConfiguration\",\n  \"description\": \"Configuration settings for creating and managing pre-provisioned snapshots for a fast-launch enabled Windows AMI.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"targetResourceCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetResourceCount\"\n        },\n        {\n          \"description\": \"The number of pre-provisioned snapshots to keep on hand for a fast-launch enabled Windows AMI.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-fast-launch-snapshot-configuration-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: FastLaunchSnapshotConfiguration
---
