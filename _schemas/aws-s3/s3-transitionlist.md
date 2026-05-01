---
description: ''
layout: schema
name: TransitionList
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-transitionlist-schema.json
slug: s3-transitionlist
source_filename: s3-transitionlist-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TransitionList\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"Date\": {},\n      \"Days\": {},\n      \"StorageClass\": {}\n    },\n    \"description\": \"Specifies when an object transitions to a specified storage class. For more information about Amazon S3 lifecycle configuration rules, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/lifecycle-transition-general-considerations.html\\\">Transitioning Objects Using Amazon S3 Lifecycle</a> in the <i>Amazon S3 User Guide</i>.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-transitionlist-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: TransitionList
---
