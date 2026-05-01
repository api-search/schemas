---
description: Provides statistical data and other information about an Amazon Web Services resource that Amazon Macie monitors and analyzes for your account.
layout: schema
name: MatchingResource
properties_list:
- description: ''
  name: matchingBucket
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-matching-resource-schema.json
slug: amazon-macie-matching-resource
source_filename: amazon-macie-matching-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-matching-resource-schema.json\",\n  \"title\": \"MatchingResource\",\n  \"description\": \"Provides statistical data and other information about an Amazon Web Services resource that Amazon Macie monitors and analyzes for your account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"matchingBucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchingBucket\"\n        },\n        {\n          \"description\": \"The details of an S3 bucket that Amazon Macie monitors and analyzes.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-matching-resource-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: MatchingResource
---
