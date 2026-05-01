---
description: A container of a key value name pair.
layout: schema
name: Tag
properties_list:
- description: Name of the object key.
  name: Key
  type: string
- description: Value of the tag.
  name: Value
  type: string
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-rest-tag-schema.json
slug: amazon-s3-rest-tag
source_filename: amazon-s3-rest-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Tag\",\n  \"type\": \"object\",\n  \"description\": \"A container of a key value name pair.\",\n  \"properties\": {\n    \"Key\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the object key.\"\n    },\n    \"Value\": {\n      \"type\": \"string\",\n      \"description\": \"Value of the tag.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-rest-tag-schema.json
tags:
- Archive
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: Tag
---
