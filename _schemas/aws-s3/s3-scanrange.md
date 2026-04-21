---
description: Specifies the byte range of the object to get the records from. A record is processed when its first byte is contained by the range. This parameter is optional, but when specified, it must not be empty. See RFC 2616, Section 14.35.1 about how to specify the start and end of the range.
layout: schema
name: ScanRange
properties_list:
- description: ''
  name: Start
  type: object
- description: ''
  name: End
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-scanrange-schema.json
slug: s3-scanrange
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ScanRange
---
