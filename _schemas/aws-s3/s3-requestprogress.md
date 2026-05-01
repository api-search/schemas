---
description: Container for specifying if periodic <code>QueryProgress</code> messages should be sent.
layout: schema
name: RequestProgress
properties_list:
- description: ''
  name: Enabled
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-requestprogress-schema.json
slug: s3-requestprogress
source_filename: s3-requestprogress-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RequestProgress\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {}\n  },\n  \"description\": \"Container for specifying if periodic <code>QueryProgress</code> messages should be sent.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-requestprogress-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: RequestProgress
---
