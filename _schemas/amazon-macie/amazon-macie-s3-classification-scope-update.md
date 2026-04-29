---
description: Specifies changes to the list of S3 buckets that are excluded from automated sensitive data discovery for an Amazon Macie account.
layout: schema
name: S3ClassificationScopeUpdate
properties_list:
- description: ''
  name: excludes
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-s3-classification-scope-update-schema.json
slug: amazon-macie-s3-classification-scope-update
source_filename: amazon-macie-s3-classification-scope-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-classification-scope-update-schema.json\",\n  \"title\": \"S3ClassificationScopeUpdate\",\n  \"description\": \"Specifies changes to the list of S3 buckets that are excluded from automated sensitive data discovery for an Amazon Macie account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"excludes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ClassificationScopeExclusionUpdate\"\n        },\n        {\n          \"description\": \"The names of the S3 buckets to add or remove from the list.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"excludes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-classification-scope-update-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: S3ClassificationScopeUpdate
---
