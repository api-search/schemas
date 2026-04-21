---
description: Requests Amazon S3 to encode the object keys in the response and specifies the encoding method to use. An object key may contain any Unicode character; however, XML 1.0 parser cannot parse some characters, such as characters with an ASCII value from 0 to 10. For characters that are not supported in XML 1.0, you can add this parameter to request that Amazon S3 encode the keys in the response.
layout: schema
name: EncodingType
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-encodingtype-schema.json
slug: s3-encodingtype
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: EncodingType
---
