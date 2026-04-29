---
description: PutClassificationExportConfigurationRequest schema from Amazon Macie API
layout: schema
name: PutClassificationExportConfigurationRequest
properties_list:
- description: ''
  name: configuration
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-put-classification-export-configuration-request-schema.json
slug: amazon-macie-put-classification-export-configuration-request
source_filename: amazon-macie-put-classification-export-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-put-classification-export-configuration-request-schema.json\",\n  \"title\": \"PutClassificationExportConfigurationRequest\",\n  \"description\": \"PutClassificationExportConfigurationRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClassificationExportConfiguration\"\n        },\n        {\n          \"description\": \"The location to store data classification results in, and the encryption settings to use when storing results in that location.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"configuration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-put-classification-export-configuration-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: PutClassificationExportConfigurationRequest
---
