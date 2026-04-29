---
description: Provides information about a type of sensitive data that was detected by a managed data identifier and produced a sensitive data finding.
layout: schema
name: DefaultDetection
properties_list:
- description: ''
  name: count
  type: object
- description: ''
  name: occurrences
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-default-detection-schema.json
slug: amazon-macie-default-detection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-default-detection-schema.json\",\n  \"title\": \"DefaultDetection\",\n  \"description\": \"Provides information about a type of sensitive data that was detected by a managed data identifier and produced a sensitive data finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of occurrences of the type of sensitive data that was detected.\"\n        }\n      ]\n    },\n    \"occurrences\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Occurrences\"\n        },\n        {\n          \"description\": \"The location of 1-15 occurrences of the sensitive data that was detected. A finding includes\
  \ location data for a maximum of 15 occurrences of sensitive data.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The type of sensitive data that was detected. For example, AWS_CREDENTIALS, PHONE_NUMBER, or ADDRESS.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-default-detection-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: DefaultDetection
---
