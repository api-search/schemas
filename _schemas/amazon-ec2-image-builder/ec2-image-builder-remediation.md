---
description: Information about how to remediate a finding.
layout: schema
name: Remediation
properties_list:
- description: ''
  name: recommendation
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-remediation-schema.json
slug: ec2-image-builder-remediation
source_filename: ec2-image-builder-remediation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-remediation-schema.json\",\n  \"title\": \"Remediation\",\n  \"description\": \"Information about how to remediate a finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"recommendation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemediationRecommendation\"\n        },\n        {\n          \"description\": \"An object that contains information about the recommended course of action to remediate the finding.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-remediation-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: Remediation
---
