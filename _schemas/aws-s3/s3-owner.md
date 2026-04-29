---
description: Container for the owner's display name and ID.
layout: schema
name: Owner
properties_list:
- description: ''
  name: DisplayName
  type: object
- description: ''
  name: ID
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-owner-schema.json
slug: s3-owner
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Owner\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DisplayName\": {},\n    \"ID\": {}\n  },\n  \"description\": \"Container for the owner's display name and ID.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-owner-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: Owner
---
