---
description: ''
layout: schema
name: InventoryConfigurationList
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-inventoryconfigurationlist-schema.json
slug: s3-inventoryconfigurationlist
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InventoryConfigurationList\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"Destination\": {},\n      \"IsEnabled\": {},\n      \"Filter\": {},\n      \"Id\": {},\n      \"IncludedObjectVersions\": {},\n      \"OptionalFields\": {},\n      \"Schedule\": {}\n    },\n    \"required\": [\n      \"Destination\",\n      \"IsEnabled\",\n      \"Id\",\n      \"IncludedObjectVersions\",\n      \"Schedule\"\n    ],\n    \"description\": \"Specifies the inventory configuration for an Amazon S3 bucket. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/API/RESTBucketGETInventoryConfig.html\\\">GET Bucket inventory</a> in the <i>Amazon S3 API Reference</i>. \"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-inventoryconfigurationlist-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: InventoryConfigurationList
---
