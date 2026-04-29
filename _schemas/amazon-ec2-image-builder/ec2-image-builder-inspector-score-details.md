---
description: Information about the factors that influenced the score that Amazon Inspector assigned for a finding.
layout: schema
name: InspectorScoreDetails
properties_list:
- description: ''
  name: adjustedCvss
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-inspector-score-details-schema.json
slug: ec2-image-builder-inspector-score-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-inspector-score-details-schema.json\",\n  \"title\": \"InspectorScoreDetails\",\n  \"description\": \"Information about the factors that influenced the score that Amazon Inspector assigned for a finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"adjustedCvss\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CvssScoreDetails\"\n        },\n        {\n          \"description\": \"An object that contains details about an adjustment that Amazon Inspector made to the CVSS score for the finding.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-inspector-score-details-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: InspectorScoreDetails
---
