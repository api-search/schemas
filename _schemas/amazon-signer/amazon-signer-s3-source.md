---
description: Information about the S3 bucket where you saved your unsigned code.
layout: schema
name: S3Source
properties_list:
- description: ''
  name: bucketName
  type: object
- description: ''
  name: key
  type: object
- description: ''
  name: version
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-s3-source-schema.json
slug: amazon-signer-s3-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-s3-source-schema.json\",\n  \"title\": \"S3Source\",\n  \"description\": \"Information about the S3 bucket where you saved your unsigned code.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketName\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"Name of the S3 bucket.\"\n        }\n      ]\n    },\n    \"key\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"Key name of the bucket object that contains your unsigned code.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"Version of your source image in your version enabled S3\
  \ bucket.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"bucketName\",\n    \"key\",\n    \"version\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-s3-source-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: S3Source
---
