---
description: ''
layout: schema
name: MetricsConfigurationList
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-metricsconfigurationlist-schema.json
slug: s3-metricsconfigurationlist
source_filename: s3-metricsconfigurationlist-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricsConfigurationList\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"Id\": {},\n      \"Filter\": {}\n    },\n    \"required\": [\n      \"Id\"\n    ],\n    \"description\": \"Specifies a metrics configuration for the CloudWatch request metrics (specified by the metrics configuration ID) from an Amazon S3 bucket. If you're updating an existing metrics configuration, note that this is a full replacement of the existing metrics configuration. If you don't include the elements you want to keep, they are erased. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/API/RESTBucketPUTMetricConfiguration.html\\\">PutBucketMetricsConfiguration</a>.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-metricsconfigurationlist-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: MetricsConfigurationList
---
