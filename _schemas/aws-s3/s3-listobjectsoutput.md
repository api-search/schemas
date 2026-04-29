---
description: ''
layout: schema
name: ListObjectsOutput
properties_list:
- description: ''
  name: IsTruncated
  type: object
- description: ''
  name: Marker
  type: object
- description: ''
  name: NextMarker
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
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-listobjectsoutput-schema.json
slug: s3-listobjectsoutput
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListObjectsOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IsTruncated\": {},\n    \"Marker\": {},\n    \"NextMarker\": {},\n    \"Contents\": {},\n    \"Name\": {},\n    \"Prefix\": {},\n    \"Delimiter\": {},\n    \"MaxKeys\": {},\n    \"CommonPrefixes\": {},\n    \"EncodingType\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-listobjectsoutput-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ListObjectsOutput
---
