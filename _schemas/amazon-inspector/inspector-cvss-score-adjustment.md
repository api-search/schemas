---
description: Details on adjustments Amazon Inspector made to the CVSS score for a finding.
layout: schema
name: CvssScoreAdjustment
properties_list:
- description: ''
  name: metric
  type: object
- description: ''
  name: reason
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-cvss-score-adjustment-schema.json
slug: inspector-cvss-score-adjustment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-cvss-score-adjustment-schema.json\",\n  \"title\": \"CvssScoreAdjustment\",\n  \"description\": \"Details on adjustments Amazon Inspector made to the CVSS score for a finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metric\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The metric used to adjust the CVSS score.\"\n        }\n      ]\n    },\n    \"reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The reason the CVSS score has been adjustment.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"metric\",\n    \"reason\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-cvss-score-adjustment-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: CvssScoreAdjustment
---
