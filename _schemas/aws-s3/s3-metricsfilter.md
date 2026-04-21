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
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: MetricsFilter
---
