---
description: The name and prefix of the S3 bucket where code signing saves your signed objects.
layout: schema
name: S3Destination
properties_list:
- description: ''
  name: bucketName
  type: object
- description: ''
  name: prefix
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-s3-destination-schema.json
slug: amazon-signer-s3-destination
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-s3-destination-schema.json\",\n  \"title\": \"S3Destination\",\n  \"description\": \"The name and prefix of the S3 bucket where code signing saves your signed objects.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketName\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"Name of the S3 bucket.\"\n        }\n      ]\n    },\n    \"prefix\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"An Amazon S3 prefix that you can use to limit responses to those that begin with the specified prefix.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-s3-destination-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: S3Destination
---
