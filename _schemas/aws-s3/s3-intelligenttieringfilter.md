---
description: The <code>Filter</code> is used to identify objects that the S3 Intelligent-Tiering configuration applies to.
layout: schema
name: IntelligentTieringFilter
properties_list:
- description: ''
  name: Prefix
  type: object
- description: A container of a key value name pair.
  name: Tag
  type: object
- description: ''
  name: And
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-intelligenttieringfilter-schema.json
slug: s3-intelligenttieringfilter
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: IntelligentTieringFilter
---
