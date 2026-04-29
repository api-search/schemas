---
description: A container for the Amazon S3 Storage Lens configuration.
layout: schema
name: StorageLensConfiguration
properties_list:
- description: A container for the Storage Lens configuration ID.
  name: Id
  type: string
- description: A container for the account-level settings for S3 Storage Lens.
  name: AccountLevel
  type: object
- description: ''
  name: Include
  type: object
- description: ''
  name: Exclude
  type: object
- description: ''
  name: DataExport
  type: object
- description: A container for whether the S3 Storage Lens configuration is enabled.
  name: IsEnabled
  type: boolean
- description: ''
  name: AwsOrg
  type: object
- description: ''
  name: StorageLensArn
  type: string
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-control-storage-lens-configuration-schema.json
slug: amazon-s3-control-storage-lens-configuration
source_filename: amazon-s3-control-storage-lens-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StorageLensConfiguration\",\n  \"type\": \"object\",\n  \"description\": \"A container for the Amazon S3 Storage Lens configuration.\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"A container for the Storage Lens configuration ID.\"\n    },\n    \"AccountLevel\": {\n      \"type\": \"object\",\n      \"description\": \"A container for the account-level settings for S3 Storage Lens.\"\n    },\n    \"Include\": {\n      \"type\": \"object\"\n    },\n    \"Exclude\": {\n      \"type\": \"object\"\n    },\n    \"DataExport\": {\n      \"type\": \"object\"\n    },\n    \"IsEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"A container for whether the S3 Storage Lens configuration is enabled.\"\n    },\n    \"AwsOrg\": {\n      \"type\": \"object\"\n    },\n    \"StorageLensArn\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-control-storage-lens-configuration-schema.json
tags:
- Archive
- AWS
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: StorageLensConfiguration
---
