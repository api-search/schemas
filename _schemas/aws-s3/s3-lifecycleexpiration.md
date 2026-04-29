---
description: Container for the expiration for the lifecycle of the object.
layout: schema
name: LifecycleExpiration
properties_list:
- description: ''
  name: Date
  type: object
- description: ''
  name: Days
  type: object
- description: ''
  name: ExpiredObjectDeleteMarker
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-lifecycleexpiration-schema.json
slug: s3-lifecycleexpiration
source_filename: s3-lifecycleexpiration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LifecycleExpiration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Date\": {},\n    \"Days\": {},\n    \"ExpiredObjectDeleteMarker\": {}\n  },\n  \"description\": \"Container for the expiration for the lifecycle of the object.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-lifecycleexpiration-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: LifecycleExpiration
---
