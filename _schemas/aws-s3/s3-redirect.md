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
source_filename: s3-redirect-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Redirect\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HostName\": {},\n    \"HttpRedirectCode\": {},\n    \"Protocol\": {},\n    \"ReplaceKeyPrefixWith\": {},\n    \"ReplaceKeyWith\": {}\n  },\n  \"description\": \"Specifies how requests are redirected. In the event of an error, you can specify a different error code to return.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-redirect-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: Redirect
---
