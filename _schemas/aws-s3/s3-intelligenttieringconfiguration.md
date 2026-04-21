---
description: <p>Specifies the S3 Intelligent-Tiering configuration for an Amazon S3 bucket.</p> <p>For information about the S3 Intelligent-Tiering storage class, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/storage-class-intro.html#sc-dynamic-data-access">Storage class for automatically optimizing frequently and infrequently accessed objects</a>.</p>
layout: schema
name: IntelligentTieringConfiguration
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Filter
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: Tierings
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-intelligenttieringconfiguration-schema.json
slug: s3-intelligenttieringconfiguration
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: IntelligentTieringConfiguration
---
