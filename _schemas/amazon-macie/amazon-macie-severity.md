---
description: Provides the numerical and qualitative representations of a finding's severity.
layout: schema
name: Severity
properties_list:
- description: ''
  name: description
  type: object
- description: ''
  name: score
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-severity-schema.json
slug: amazon-macie-severity
source_filename: amazon-macie-severity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-severity-schema.json\",\n  \"title\": \"Severity\",\n  \"description\": \"Provides the numerical and qualitative representations of a finding's severity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SeverityDescription\"\n        },\n        {\n          \"description\": \"The qualitative representation of the finding's severity, ranging from Low (least severe) to High (most severe).\"\n        }\n      ]\n    },\n    \"score\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The numerical representation of the finding's severity, ranging from 1 (least severe) to 3 (most severe).\"\n        }\n      ]\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-severity-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: Severity
---
