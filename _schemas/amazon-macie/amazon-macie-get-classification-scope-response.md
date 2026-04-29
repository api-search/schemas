---
description: GetClassificationScopeResponse schema from Amazon Macie API
layout: schema
name: GetClassificationScopeResponse
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: s3
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-classification-scope-response-schema.json
slug: amazon-macie-get-classification-scope-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-classification-scope-response-schema.json\",\n  \"title\": \"GetClassificationScopeResponse\",\n  \"description\": \"GetClassificationScopeResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClassificationScopeId\"\n        },\n        {\n          \"description\": \"The unique identifier for the classification scope.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClassificationScopeName\"\n        },\n        {\n          \"description\": \"The name of the classification scope: automated-sensitive-data-discovery.\"\n        }\n      ]\n    },\n    \"s3\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/S3ClassificationScope\"\n        },\n        {\n          \"description\": \"The S3 buckets that are excluded from automated sensitive data discovery.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-classification-scope-response-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetClassificationScopeResponse
---
