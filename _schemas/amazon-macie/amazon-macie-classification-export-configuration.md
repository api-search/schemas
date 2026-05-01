---
description: Specifies where to store data classification results, and the encryption settings to use when storing results in that location. The location must be an S3 bucket.
layout: schema
name: ClassificationExportConfiguration
properties_list:
- description: ''
  name: s3Destination
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-classification-export-configuration-schema.json
slug: amazon-macie-classification-export-configuration
source_filename: amazon-macie-classification-export-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-classification-export-configuration-schema.json\",\n  \"title\": \"ClassificationExportConfiguration\",\n  \"description\": \"Specifies where to store data classification results, and the encryption settings to use when storing results in that location. The location must be an S3 bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s3Destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Destination\"\n        },\n        {\n          \"description\": \"The S3 bucket to store data classification results in, and the encryption settings to use when storing results in that bucket.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-classification-export-configuration-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ClassificationExportConfiguration
---
