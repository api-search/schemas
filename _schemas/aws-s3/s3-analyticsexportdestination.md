---
description: Where to publish the analytics results.
layout: schema
name: AnalyticsExportDestination
properties_list:
- description: ''
  name: S3BucketDestination
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-analyticsexportdestination-schema.json
slug: s3-analyticsexportdestination
source_filename: s3-analyticsexportdestination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AnalyticsExportDestination\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3BucketDestination\": {}\n  },\n  \"required\": [\n    \"S3BucketDestination\"\n  ],\n  \"description\": \"Where to publish the analytics results.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-analyticsexportdestination-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: AnalyticsExportDestination
---
