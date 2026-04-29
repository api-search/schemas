---
description: GetClassificationExportConfigurationResponse schema from Amazon Macie API
layout: schema
name: GetClassificationExportConfigurationResponse
properties_list:
- description: ''
  name: configuration
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-classification-export-configuration-response-schema.json
slug: amazon-macie-get-classification-export-configuration-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-classification-export-configuration-response-schema.json\",\n  \"title\": \"GetClassificationExportConfigurationResponse\",\n  \"description\": \"GetClassificationExportConfigurationResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClassificationExportConfiguration\"\n        },\n        {\n          \"description\": \"The location where data classification results are stored, and the encryption settings that are used when storing results in that location.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-classification-export-configuration-response-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetClassificationExportConfigurationResponse
---
