---
description: Provides information about the resources that a finding applies to.
layout: schema
name: ResourcesAffected
properties_list:
- description: ''
  name: s3Bucket
  type: object
- description: ''
  name: s3Object
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-resources-affected-schema.json
slug: amazon-macie-resources-affected
source_filename: amazon-macie-resources-affected-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-resources-affected-schema.json\",\n  \"title\": \"ResourcesAffected\",\n  \"description\": \"Provides information about the resources that a finding applies to.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s3Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Bucket\"\n        },\n        {\n          \"description\": \"The details of the S3 bucket that the finding applies to.\"\n        }\n      ]\n    },\n    \"s3Object\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Object\"\n        },\n        {\n          \"description\": \"The details of the S3 object that the finding applies to.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-resources-affected-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ResourcesAffected
---
