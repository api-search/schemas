---
description: Specifies the names of the S3 buckets that are excluded from automated sensitive data discovery.
layout: schema
name: S3ClassificationScopeExclusion
properties_list:
- description: ''
  name: bucketNames
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-s3-classification-scope-exclusion-schema.json
slug: amazon-macie-s3-classification-scope-exclusion
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-classification-scope-exclusion-schema.json\",\n  \"title\": \"S3ClassificationScopeExclusion\",\n  \"description\": \"Specifies the names of the S3 buckets that are excluded from automated sensitive data discovery.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfS3BucketName\"\n        },\n        {\n          \"description\": \"An array of strings, one for each S3 bucket that is excluded. Each string is the full name of an excluded bucket.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"bucketNames\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-classification-scope-exclusion-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: S3ClassificationScopeExclusion
---
