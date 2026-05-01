---
description: Container for all error elements.
layout: schema
name: Error
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: VersionId
  type: object
- description: ''
  name: Code
  type: object
- description: ''
  name: Message
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-error-schema.json
slug: s3-error
source_filename: s3-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {},\n    \"VersionId\": {},\n    \"Code\": {},\n    \"Message\": {}\n  },\n  \"description\": \"Container for all error elements.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-error-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: Error
---
