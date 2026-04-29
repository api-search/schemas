---
description: Provides information about an S3 object that lists specific text to ignore.
layout: schema
name: S3WordsList
properties_list:
- description: ''
  name: bucketName
  type: object
- description: ''
  name: objectKey
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-s3-words-list-schema.json
slug: amazon-macie-s3-words-list
source_filename: amazon-macie-s3-words-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-words-list-schema.json\",\n  \"title\": \"S3WordsList\",\n  \"description\": \"Provides information about an S3 object that lists specific text to ignore.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin3Max255PatternAZaZ093255\"\n        },\n        {\n          \"description\": \"The full name of the S3 bucket that contains the object.\"\n        }\n      ]\n    },\n    \"objectKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max1024PatternSS\"\n        },\n        {\n          \"description\": \"The full name (key) of the object.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"bucketName\",\n    \"objectKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-words-list-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: S3WordsList
---
