---
description: Confirms that the requester knows that they will be charged for the request. Bucket owners need not specify this parameter in their requests. For information about downloading objects from Requester Pays buckets, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/ObjectsinRequesterPaysBuckets.html">Downloading Objects in Requester Pays Buckets</a> in the <i>Amazon S3 User Guide</i>.
layout: schema
name: RequestPayer
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-requestpayer-schema.json
slug: s3-requestpayer
source_filename: s3-requestpayer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RequestPayer\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"requester\"\n  ],\n  \"description\": \"Confirms that the requester knows that they will be charged for the request. Bucket owners need not specify this parameter in their requests. For information about downloading objects from Requester Pays buckets, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/ObjectsinRequesterPaysBuckets.html\\\">Downloading Objects in Requester Pays Buckets</a> in the <i>Amazon S3 User Guide</i>.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-requestpayer-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: RequestPayer
---
