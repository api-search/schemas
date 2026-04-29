---
description: ''
layout: schema
name: IntelligentTieringConfigurationList
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-intelligenttieringconfigurationlist-schema.json
slug: s3-intelligenttieringconfigurationlist
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IntelligentTieringConfigurationList\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"Id\": {},\n      \"Filter\": {},\n      \"Status\": {},\n      \"Tierings\": {}\n    },\n    \"required\": [\n      \"Id\",\n      \"Status\",\n      \"Tierings\"\n    ],\n    \"description\": \"<p>Specifies the S3 Intelligent-Tiering configuration for an Amazon S3 bucket.</p> <p>For information about the S3 Intelligent-Tiering storage class, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/storage-class-intro.html#sc-dynamic-data-access\\\">Storage class for automatically optimizing frequently and infrequently accessed objects</a>.</p>\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-intelligenttieringconfigurationlist-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: IntelligentTieringConfigurationList
---
