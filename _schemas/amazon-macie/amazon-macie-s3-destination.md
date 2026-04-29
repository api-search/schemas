---
description: Specifies an S3 bucket to store data classification results in, and the encryption settings to use when storing results in that bucket.
layout: schema
name: S3Destination
properties_list:
- description: ''
  name: bucketName
  type: object
- description: ''
  name: keyPrefix
  type: object
- description: ''
  name: kmsKeyArn
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-s3-destination-schema.json
slug: amazon-macie-s3-destination
source_filename: amazon-macie-s3-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-destination-schema.json\",\n  \"title\": \"S3Destination\",\n  \"description\": \"Specifies an S3 bucket to store data classification results in, and the encryption settings to use when storing results in that bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the bucket.\"\n        }\n      ]\n    },\n    \"keyPrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The path prefix to use in the path to the location in the bucket. This prefix specifies where to store classification results in the bucket.\"\n        }\n\
  \      ]\n    },\n    \"kmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the customer managed KMS key to use for encryption of the results. This must be the ARN of an existing, symmetric encryption KMS key that's in the same Amazon Web Services Region as the bucket.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"bucketName\",\n    \"kmsKeyArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-destination-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: S3Destination
---
