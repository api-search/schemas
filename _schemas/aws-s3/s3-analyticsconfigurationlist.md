---
description: ''
layout: schema
name: AnalyticsConfigurationList
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-analyticsconfigurationlist-schema.json
slug: s3-analyticsconfigurationlist
source_filename: s3-analyticsconfigurationlist-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AnalyticsConfigurationList\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"Id\": {},\n      \"Filter\": {},\n      \"StorageClassAnalysis\": {}\n    },\n    \"required\": [\n      \"Id\",\n      \"StorageClassAnalysis\"\n    ],\n    \"description\": \"Specifies the configuration and any analyses for the analytics filter of an Amazon S3 bucket.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-analyticsconfigurationlist-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: AnalyticsConfigurationList
---
