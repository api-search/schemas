---
description: ''
layout: schema
name: TieringList
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-tieringlist-schema.json
slug: s3-tieringlist
source_filename: s3-tieringlist-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TieringList\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"Days\": {},\n      \"AccessTier\": {}\n    },\n    \"required\": [\n      \"Days\",\n      \"AccessTier\"\n    ],\n    \"description\": \"The S3 Intelligent-Tiering storage class is designed to optimize storage costs by automatically moving data to the most cost-effective storage access tier, without additional operational overhead.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-tieringlist-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: TieringList
---
