---
description: Provides information about a custom data identifier that produced a sensitive data finding, and the sensitive data that it detected for the finding.
layout: schema
name: CustomDetection
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: count
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: occurrences
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-custom-detection-schema.json
slug: amazon-macie-custom-detection
source_filename: amazon-macie-custom-detection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-custom-detection-schema.json\",\n  \"title\": \"CustomDetection\",\n  \"description\": \"Provides information about a custom data identifier that produced a sensitive data finding, and the sensitive data that it detected for the finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the custom data identifier.\"\n        }\n      ]\n    },\n    \"count\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of occurrences of the sensitive data that the custom data identifier detected.\"\n        }\n      ]\n  \
  \  },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the custom data identifier.\"\n        }\n      ]\n    },\n    \"occurrences\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Occurrences\"\n        },\n        {\n          \"description\": \"The location of 1-15 occurrences of the sensitive data that the custom data identifier detected. A finding includes location data for a maximum of 15 occurrences of sensitive data.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-custom-detection-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: CustomDetection
---
