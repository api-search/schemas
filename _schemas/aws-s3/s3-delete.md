---
description: Container for the objects to delete.
layout: schema
name: Delete
properties_list:
- description: ''
  name: Objects
  type: object
- description: ''
  name: Quiet
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-delete-schema.json
slug: s3-delete
source_filename: s3-delete-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Delete\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Objects\": {},\n    \"Quiet\": {}\n  },\n  \"required\": [\n    \"Objects\"\n  ],\n  \"description\": \"Container for the objects to delete.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-delete-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: Delete
---
