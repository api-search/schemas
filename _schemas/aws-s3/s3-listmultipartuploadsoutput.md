---
description: ''
layout: schema
name: ListMultipartUploadsOutput
properties_list:
- description: ''
  name: Bucket
  type: object
- description: ''
  name: KeyMarker
  type: object
- description: ''
  name: UploadIdMarker
  type: object
- description: ''
  name: NextKeyMarker
  type: object
- description: ''
  name: Prefix
  type: object
- description: ''
  name: Delimiter
  type: object
- description: ''
  name: NextUploadIdMarker
  type: object
- description: ''
  name: MaxUploads
  type: object
- description: ''
  name: IsTruncated
  type: object
- description: ''
  name: Uploads
  type: object
- description: ''
  name: CommonPrefixes
  type: object
- description: ''
  name: EncodingType
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-listmultipartuploadsoutput-schema.json
slug: s3-listmultipartuploadsoutput
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListMultipartUploadsOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bucket\": {},\n    \"KeyMarker\": {},\n    \"UploadIdMarker\": {},\n    \"NextKeyMarker\": {},\n    \"Prefix\": {},\n    \"Delimiter\": {},\n    \"NextUploadIdMarker\": {},\n    \"MaxUploads\": {},\n    \"IsTruncated\": {},\n    \"Uploads\": {},\n    \"CommonPrefixes\": {},\n    \"EncodingType\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-listmultipartuploadsoutput-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ListMultipartUploadsOutput
---
