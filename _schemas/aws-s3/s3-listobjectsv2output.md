---
description: ''
layout: schema
name: ListObjectsV2Output
properties_list:
- description: ''
  name: IsTruncated
  type: object
- description: ''
  name: Contents
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Prefix
  type: object
- description: ''
  name: Delimiter
  type: object
- description: ''
  name: MaxKeys
  type: object
- description: ''
  name: CommonPrefixes
  type: object
- description: ''
  name: EncodingType
  type: object
- description: ''
  name: KeyCount
  type: object
- description: ''
  name: ContinuationToken
  type: object
- description: ''
  name: NextContinuationToken
  type: object
- description: ''
  name: StartAfter
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-listobjectsv2output-schema.json
slug: s3-listobjectsv2output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListObjectsV2Output\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IsTruncated\": {},\n    \"Contents\": {},\n    \"Name\": {},\n    \"Prefix\": {},\n    \"Delimiter\": {},\n    \"MaxKeys\": {},\n    \"CommonPrefixes\": {},\n    \"EncodingType\": {},\n    \"KeyCount\": {},\n    \"ContinuationToken\": {},\n    \"NextContinuationToken\": {},\n    \"StartAfter\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-listobjectsv2output-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ListObjectsV2Output
---
