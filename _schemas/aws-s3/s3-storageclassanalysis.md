---
description: Specifies data related to access patterns to be collected and made available to analyze the tradeoffs between different storage classes for an Amazon S3 bucket.
layout: schema
name: StorageClassAnalysis
properties_list:
- description: ''
  name: DataExport
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-storageclassanalysis-schema.json
slug: s3-storageclassanalysis
source_filename: s3-storageclassanalysis-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StorageClassAnalysis\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DataExport\": {}\n  },\n  \"description\": \"Specifies data related to access patterns to be collected and made available to analyze the tradeoffs between different storage classes for an Amazon S3 bucket.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-storageclassanalysis-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: StorageClassAnalysis
---
