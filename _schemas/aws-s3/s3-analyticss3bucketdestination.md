---
description: Contains information about where to publish the analytics results.
layout: schema
name: AnalyticsS3BucketDestination
properties_list:
- description: ''
  name: Format
  type: object
- description: ''
  name: BucketAccountId
  type: object
- description: ''
  name: Bucket
  type: object
- description: ''
  name: Prefix
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-analyticss3bucketdestination-schema.json
slug: s3-analyticss3bucketdestination
source_filename: s3-analyticss3bucketdestination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AnalyticsS3BucketDestination\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Format\": {},\n    \"BucketAccountId\": {},\n    \"Bucket\": {},\n    \"Prefix\": {}\n  },\n  \"required\": [\n    \"Format\",\n    \"Bucket\"\n  ],\n  \"description\": \"Contains information about where to publish the analytics results.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-analyticss3bucketdestination-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: AnalyticsS3BucketDestination
---
