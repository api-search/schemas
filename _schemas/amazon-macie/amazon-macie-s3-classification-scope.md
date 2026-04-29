---
description: Specifies the S3 buckets that are excluded from automated sensitive data discovery for an Amazon Macie account.
layout: schema
name: S3ClassificationScope
properties_list:
- description: ''
  name: excludes
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-s3-classification-scope-schema.json
slug: amazon-macie-s3-classification-scope
source_filename: amazon-macie-s3-classification-scope-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-classification-scope-schema.json\",\n  \"title\": \"S3ClassificationScope\",\n  \"description\": \"Specifies the S3 buckets that are excluded from automated sensitive data discovery for an Amazon Macie account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"excludes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ClassificationScopeExclusion\"\n        },\n        {\n          \"description\": \"The S3 buckets that are excluded.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"excludes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-classification-scope-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: S3ClassificationScope
---
