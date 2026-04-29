---
description: CvssScoreAdjustmentList schema
layout: schema
name: CvssScoreAdjustmentList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-cvss-score-adjustment-list-schema.json
slug: inspector-cvss-score-adjustment-list
source_filename: inspector-cvss-score-adjustment-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-cvss-score-adjustment-list-schema.json\",\n  \"title\": \"CvssScoreAdjustmentList\",\n  \"description\": \"CvssScoreAdjustmentList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"metric\",\n      \"reason\"\n    ],\n    \"properties\": {\n      \"metric\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/NonEmptyString\"\n          },\n          {\n            \"description\": \"The metric used to adjust the CVSS score.\"\n          }\n        ]\n      },\n      \"reason\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/NonEmptyString\"\n          },\n          {\n            \"description\": \"The reason the CVSS score has been adjustment.\"\n          }\n       \
  \ ]\n      }\n    },\n    \"description\": \"Details on adjustments Amazon Inspector made to the CVSS score for a finding.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-cvss-score-adjustment-list-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: CvssScoreAdjustmentList
---
