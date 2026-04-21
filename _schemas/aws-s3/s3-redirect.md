---
description: Specifies how requests are redirected. In the event of an error, you can specify a different error code to return.
layout: schema
name: Redirect
properties_list:
- description: ''
  name: HostName
  type: object
- description: ''
  name: HttpRedirectCode
  type: object
- description: ''
  name: Protocol
  type: object
- description: ''
  name: ReplaceKeyPrefixWith
  type: object
- description: ''
  name: ReplaceKeyWith
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-redirect-schema.json
slug: s3-redirect
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: Redirect
---
