---
description: ''
layout: schema
name: ListObjectVersionsOutput
properties_list:
- description: ''
  name: IsTruncated
  type: object
- description: ''
  name: KeyMarker
  type: object
- description: ''
  name: VersionIdMarker
  type: object
- description: ''
  name: NextKeyMarker
  type: object
- description: ''
  name: NextVersionIdMarker
  type: object
- description: ''
  name: Versions
  type: object
- description: ''
  name: DeleteMarkers
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
schema_file: json-schema/s3-listobjectversionsoutput-schema.json
slug: s3-listobjectversionsoutput
source_filename: s3-listobjectversionsoutput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListObjectVersionsOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IsTruncated\": {},\n    \"KeyMarker\": {},\n    \"VersionIdMarker\": {},\n    \"NextKeyMarker\": {},\n    \"NextVersionIdMarker\": {},\n    \"Versions\": {},\n    \"DeleteMarkers\": {},\n    \"Name\": {},\n    \"Prefix\": {},\n    \"Delimiter\": {},\n    \"MaxKeys\": {},\n    \"CommonPrefixes\": {},\n    \"EncodingType\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-listobjectversionsoutput-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ListObjectVersionsOutput
---
