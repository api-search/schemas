---
description: A container specifying S3 Replication Time Control (S3 RTC) related information, including whether S3 RTC is enabled and the time when all objects and operations on objects must be replicated. Must be specified together with a <code>Metrics</code> block.
layout: schema
name: ReplicationTime
properties_list:
- description: ''
  name: Status
  type: object
- description: ''
  name: Time
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-replicationtime-schema.json
slug: s3-replicationtime
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ReplicationTime
---
