---
description: Represents an Amazon Security Lake data lake configuration.
layout: schema
name: DataLake
properties_list:
- description: The ARN of the data lake.
  name: dataLakeArn
  type: string
- description: The AWS region where the data lake is configured.
  name: region
  type: string
- description: The current status of the data lake.
  name: status
  type: string
- description: The encryption configuration for the data lake.
  name: encryptionConfiguration
  type: object
- description: The lifecycle configuration for the data lake.
  name: lifecycleConfiguration
  type: object
- description: The ARN of the S3 bucket where security data is stored.
  name: s3BucketArn
  type: string
provider_name: Amazon Security Lake
provider_slug: amazon-security-lake
schema_file: json-schema/amazon-security-lake-data-lake-schema.json
slug: amazon-security-lake-data-lake
source_filename: amazon-security-lake-data-lake-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-security-lake/refs/heads/main/json-schema/amazon-security-lake-data-lake-schema.json\",\n  \"title\": \"DataLake\",\n  \"description\": \"Represents an Amazon Security Lake data lake configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dataLakeArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the data lake.\",\n      \"example\": \"arn:aws:securitylake:us-east-1:123456789012:data-lake/default\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS region where the data lake is configured.\",\n      \"example\": \"us-east-1\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the data lake.\",\n      \"enum\": [\n        \"INITIALIZED\",\n        \"PENDING\",\n        \"COMPLETED\",\n        \"FAILED\"\n     \
  \ ],\n      \"example\": \"INITIALIZED\"\n    },\n    \"encryptionConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"The encryption configuration for the data lake.\",\n      \"properties\": {\n        \"kmsKeyId\": {\n          \"type\": \"string\",\n          \"description\": \"The KMS key ID for encryption.\"\n        }\n      }\n    },\n    \"lifecycleConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"The lifecycle configuration for the data lake.\",\n      \"properties\": {\n        \"expiration\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"days\": {\n              \"type\": \"integer\"\n            }\n          }\n        },\n        \"transitions\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\"\n          }\n        }\n      }\n    },\n    \"s3BucketArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the S3 bucket where security data\
  \ is stored.\",\n      \"example\": \"arn:aws:s3:::aws-security-data-lake-us-east-1-abc123\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-security-lake/refs/heads/main/json-schema/amazon-security-lake-data-lake-schema.json
tags:
- Data Lake
- Security
- SIEM
- Threat Detection
title: DataLake
---
