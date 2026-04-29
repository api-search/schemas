---
description: Information about the delete marker.
layout: schema
name: DeleteMarkerEntry
properties_list:
- description: ''
  name: Owner
  type: object
- description: ''
  name: Key
  type: object
- description: ''
  name: VersionId
  type: object
- description: ''
  name: IsLatest
  type: object
- description: ''
  name: LastModified
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-deletemarkerentry-schema.json
slug: s3-deletemarkerentry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeleteMarkerEntry\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Owner\": {},\n    \"Key\": {},\n    \"VersionId\": {},\n    \"IsLatest\": {},\n    \"LastModified\": {}\n  },\n  \"description\": \"Information about the delete marker.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-deletemarkerentry-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: DeleteMarkerEntry
---
