---
description: The S3 Intelligent-Tiering storage class is designed to optimize storage costs by automatically moving data to the most cost-effective storage access tier, without additional operational overhead.
layout: schema
name: Tiering
properties_list:
- description: ''
  name: Days
  type: object
- description: ''
  name: AccessTier
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-tiering-schema.json
slug: s3-tiering
source_filename: s3-tiering-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Tiering\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Days\": {},\n    \"AccessTier\": {}\n  },\n  \"required\": [\n    \"Days\",\n    \"AccessTier\"\n  ],\n  \"description\": \"The S3 Intelligent-Tiering storage class is designed to optimize storage costs by automatically moving data to the most cost-effective storage access tier, without additional operational overhead.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-tiering-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: Tiering
---
