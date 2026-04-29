---
description: ''
layout: schema
name: StorageLocationS3
properties_list:
- description: Specifies the case-sensitive Amazon Resource Name (ARN) of the AWS identity and access management (IAM) role that grants privileges on the S3 bucket containing your data files.
  name: storage_aws_role_arn
  type: string
- description: Specifies the base URL for your cloud storage location.
  name: storage_base_url
  type: string
- description: Optionally specifies an external ID that Snowflake uses to establish a trust relationship with AWS.
  name: storage_aws_external_id
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/external-volume-storage-location-s3-schema.json
slug: external-volume-storage-location-s3
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StorageLocationS3\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"storage_aws_role_arn\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the case-sensitive Amazon Resource Name (ARN) of the AWS identity and access management (IAM) role that grants privileges on the S3 bucket containing your data files.\"\n    },\n    \"storage_base_url\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the base URL for your cloud storage location.\"\n    },\n    \"storage_aws_external_id\": {\n      \"type\": \"string\",\n      \"description\": \"Optionally specifies an external ID that Snowflake uses to establish a trust relationship with AWS.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/external-volume-storage-location-s3-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: StorageLocationS3
---
