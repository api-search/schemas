---
description: Container for all (if there are any) keys between Prefix and the next occurrence of the string specified by a delimiter. CommonPrefixes lists keys that act like subdirectories in the directory specified by Prefix. For example, if the prefix is notes/ and the delimiter is a slash (/) as in notes/summer/july, the common prefix is notes/summer/.
layout: schema
name: CommonPrefix
properties_list:
- description: ''
  name: Prefix
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-commonprefix-schema.json
slug: s3-commonprefix
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: CommonPrefix
---
