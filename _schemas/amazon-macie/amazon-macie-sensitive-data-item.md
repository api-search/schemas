---
description: Provides information about the category, types, and occurrences of sensitive data that produced a sensitive data finding.
layout: schema
name: SensitiveDataItem
properties_list:
- description: ''
  name: category
  type: object
- description: ''
  name: detections
  type: object
- description: ''
  name: totalCount
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-sensitive-data-item-schema.json
slug: amazon-macie-sensitive-data-item
source_filename: amazon-macie-sensitive-data-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-sensitive-data-item-schema.json\",\n  \"title\": \"SensitiveDataItem\",\n  \"description\": \"Provides information about the category, types, and occurrences of sensitive data that produced a sensitive data finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveDataItemCategory\"\n        },\n        {\n          \"description\": \"The category of sensitive data that was detected. For example: CREDENTIALS, for credentials data such as private keys or Amazon Web Services secret access keys; FINANCIAL_INFORMATION, for financial data such as credit card numbers; or, PERSONAL_INFORMATION, for personal health information, such as health insurance identification numbers, or personally identifiable\
  \ information, such as passport numbers.\"\n        }\n      ]\n    },\n    \"detections\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultDetections\"\n        },\n        {\n          \"description\": \"An array of objects, one for each type of sensitive data that was detected. Each object reports the number of occurrences of a specific type of sensitive data that was detected, and the location of up to 15 of those occurrences.\"\n        }\n      ]\n    },\n    \"totalCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of occurrences of the sensitive data that was detected.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-sensitive-data-item-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: SensitiveDataItem
---
