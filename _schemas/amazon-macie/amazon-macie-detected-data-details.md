---
description: Specifies 1-10 occurrences of a specific type of sensitive data reported by a finding.
layout: schema
name: DetectedDataDetails
properties_list:
- description: ''
  name: value
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-detected-data-details-schema.json
slug: amazon-macie-detected-data-details
source_filename: amazon-macie-detected-data-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-detected-data-details-schema.json\",\n  \"title\": \"DetectedDataDetails\",\n  \"description\": \"Specifies 1-10 occurrences of a specific type of sensitive data reported by a finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max128\"\n        },\n        {\n          \"description\": \"An occurrence of the specified type of sensitive data. Each occurrence can contain 1-128 characters.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-detected-data-details-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: DetectedDataDetails
---
