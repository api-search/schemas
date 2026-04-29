---
description: Specifies a metrics configuration filter. The metrics configuration only includes objects that meet the filter's criteria. A filter must be a prefix, an object tag, an access point ARN, or a conjunction (MetricsAndOperator). For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutBucketMetricsConfiguration.html">PutBucketMetricsConfiguration</a>.
layout: schema
name: MetricsFilter
properties_list:
- description: ''
  name: Prefix
  type: object
- description: ''
  name: Tag
  type: object
- description: ''
  name: AccessPointArn
  type: object
- description: ''
  name: And
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-metricsfilter-schema.json
slug: s3-metricsfilter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricsFilter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Prefix\": {},\n    \"Tag\": {},\n    \"AccessPointArn\": {},\n    \"And\": {}\n  },\n  \"description\": \"Specifies a metrics configuration filter. The metrics configuration only includes objects that meet the filter's criteria. A filter must be a prefix, an object tag, an access point ARN, or a conjunction (MetricsAndOperator). For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutBucketMetricsConfiguration.html\\\">PutBucketMetricsConfiguration</a>.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-metricsfilter-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: MetricsFilter
---
