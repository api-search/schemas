---
description: Details about an adjustment that Amazon Inspector made to the CVSS score for a finding.
layout: schema
name: CvssScoreAdjustment
properties_list:
- description: ''
  name: metric
  type: object
- description: ''
  name: reason
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-cvss-score-adjustment-schema.json
slug: ec2-image-builder-cvss-score-adjustment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-cvss-score-adjustment-schema.json\",\n  \"title\": \"CvssScoreAdjustment\",\n  \"description\": \"Details about an adjustment that Amazon Inspector made to the CVSS score for a finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metric\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The metric that Amazon Inspector used to adjust the CVSS score.\"\n        }\n      ]\n    },\n    \"reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The reason for the CVSS score adjustment.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-cvss-score-adjustment-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: CvssScoreAdjustment
---
