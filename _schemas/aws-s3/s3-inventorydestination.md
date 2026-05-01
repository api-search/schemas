---
description: Specifies the inventory configuration for an Amazon S3 bucket.
layout: schema
name: InventoryDestination
properties_list:
- description: ''
  name: S3BucketDestination
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-inventorydestination-schema.json
slug: s3-inventorydestination
source_filename: s3-inventorydestination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InventoryDestination\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3BucketDestination\": {}\n  },\n  \"required\": [\n    \"S3BucketDestination\"\n  ],\n  \"description\": \"Specifies the inventory configuration for an Amazon S3 bucket.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-inventorydestination-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: InventoryDestination
---
