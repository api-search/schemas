---
description: Container for the stats details.
layout: schema
name: Stats
properties_list:
- description: ''
  name: BytesScanned
  type: object
- description: ''
  name: BytesProcessed
  type: object
- description: ''
  name: BytesReturned
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-stats-schema.json
slug: s3-stats
source_filename: s3-stats-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Stats\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BytesScanned\": {},\n    \"BytesProcessed\": {},\n    \"BytesReturned\": {}\n  },\n  \"description\": \"Container for the stats details.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-stats-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: Stats
---
