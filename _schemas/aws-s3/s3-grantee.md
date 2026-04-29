---
description: Container for the person being granted permissions.
layout: schema
name: Grantee
properties_list:
- description: ''
  name: DisplayName
  type: object
- description: ''
  name: EmailAddress
  type: object
- description: ''
  name: ID
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: URI
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-grantee-schema.json
slug: s3-grantee
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Grantee\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DisplayName\": {},\n    \"EmailAddress\": {},\n    \"ID\": {},\n    \"Type\": {},\n    \"URI\": {}\n  },\n  \"required\": [\n    \"Type\"\n  ],\n  \"description\": \"Container for the person being granted permissions.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-grantee-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: Grantee
---
