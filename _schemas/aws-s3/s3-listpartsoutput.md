---
description: ''
layout: schema
name: ListPartsOutput
properties_list:
- description: ''
  name: Bucket
  type: object
- description: ''
  name: Key
  type: object
- description: ''
  name: UploadId
  type: object
- description: ''
  name: PartNumberMarker
  type: object
- description: ''
  name: NextPartNumberMarker
  type: object
- description: ''
  name: MaxParts
  type: object
- description: ''
  name: IsTruncated
  type: object
- description: ''
  name: Parts
  type: object
- description: ''
  name: Initiator
  type: object
- description: ''
  name: Owner
  type: object
- description: ''
  name: StorageClass
  type: object
- description: ''
  name: ChecksumAlgorithm
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-listpartsoutput-schema.json
slug: s3-listpartsoutput
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListPartsOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bucket\": {},\n    \"Key\": {},\n    \"UploadId\": {},\n    \"PartNumberMarker\": {},\n    \"NextPartNumberMarker\": {},\n    \"MaxParts\": {},\n    \"IsTruncated\": {},\n    \"Parts\": {},\n    \"Initiator\": {},\n    \"Owner\": {},\n    \"StorageClass\": {},\n    \"ChecksumAlgorithm\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-listpartsoutput-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ListPartsOutput
---
