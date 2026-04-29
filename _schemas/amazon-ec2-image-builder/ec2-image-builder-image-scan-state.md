---
description: Shows the vulnerability scan status for a specific image, and the reason for that status.
layout: schema
name: ImageScanState
properties_list:
- description: ''
  name: status
  type: object
- description: ''
  name: reason
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-image-scan-state-schema.json
slug: ec2-image-builder-image-scan-state
source_filename: ec2-image-builder-image-scan-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-scan-state-schema.json\",\n  \"title\": \"ImageScanState\",\n  \"description\": \"Shows the vulnerability scan status for a specific image, and the reason for that status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageScanStatus\"\n        },\n        {\n          \"description\": \"The current state of vulnerability scans for the image.\"\n        }\n      ]\n    },\n    \"reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The reason for the scan status for the image.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-scan-state-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ImageScanState
---
