---
description: Container element that identifies who initiated the multipart upload.
layout: schema
name: Initiator
properties_list:
- description: ''
  name: ID
  type: object
- description: ''
  name: DisplayName
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-initiator-schema.json
slug: s3-initiator
source_filename: s3-initiator-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Initiator\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ID\": {},\n    \"DisplayName\": {}\n  },\n  \"description\": \"Container element that identifies who initiated the multipart upload. \"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-initiator-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: Initiator
---
