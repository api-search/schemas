---
description: Container for data related to the storage class analysis for an Amazon S3 bucket for export.
layout: schema
name: StorageClassAnalysisDataExport
properties_list:
- description: ''
  name: OutputSchemaVersion
  type: object
- description: ''
  name: Destination
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-storageclassanalysisdataexport-schema.json
slug: s3-storageclassanalysisdataexport
source_filename: s3-storageclassanalysisdataexport-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StorageClassAnalysisDataExport\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OutputSchemaVersion\": {},\n    \"Destination\": {}\n  },\n  \"required\": [\n    \"OutputSchemaVersion\",\n    \"Destination\"\n  ],\n  \"description\": \"Container for data related to the storage class analysis for an Amazon S3 bucket for export.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-storageclassanalysisdataexport-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: StorageClassAnalysisDataExport
---
