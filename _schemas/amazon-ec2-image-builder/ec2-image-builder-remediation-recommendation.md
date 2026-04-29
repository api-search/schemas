---
description: Details about the recommended course of action to remediate the finding.
layout: schema
name: RemediationRecommendation
properties_list:
- description: ''
  name: text
  type: object
- description: ''
  name: url
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-remediation-recommendation-schema.json
slug: ec2-image-builder-remediation-recommendation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-remediation-recommendation-schema.json\",\n  \"title\": \"RemediationRecommendation\",\n  \"description\": \"Details about the recommended course of action to remediate the finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"text\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The recommended course of action to remediate the finding.\"\n        }\n      ]\n    },\n    \"url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"A link to more information about the recommended remediation for this vulnerability.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-remediation-recommendation-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: RemediationRecommendation
---
