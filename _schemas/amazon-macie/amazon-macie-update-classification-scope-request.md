---
description: UpdateClassificationScopeRequest schema from Amazon Macie API
layout: schema
name: UpdateClassificationScopeRequest
properties_list:
- description: ''
  name: s3
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-update-classification-scope-request-schema.json
slug: amazon-macie-update-classification-scope-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-update-classification-scope-request-schema.json\",\n  \"title\": \"UpdateClassificationScopeRequest\",\n  \"description\": \"UpdateClassificationScopeRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s3\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ClassificationScopeUpdate\"\n        },\n        {\n          \"description\": \"The S3 buckets to add or remove from the exclusion list defined by the classification scope.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-update-classification-scope-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: UpdateClassificationScopeRequest
---
