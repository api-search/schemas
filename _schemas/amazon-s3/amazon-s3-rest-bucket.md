---
description: In terms of implementation, a Bucket is a resource.
layout: schema
name: Bucket
properties_list:
- description: The name of the bucket.
  name: Name
  type: string
- description: Date the bucket was created.
  name: CreationDate
  type: string
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-rest-bucket-schema.json
slug: amazon-s3-rest-bucket
source_filename: amazon-s3-rest-bucket-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Bucket\",\n  \"type\": \"object\",\n  \"description\": \"In terms of implementation, a Bucket is a resource.\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the bucket.\"\n    },\n    \"CreationDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date the bucket was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-rest-bucket-schema.json
tags:
- Archive
- AWS
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: Bucket
---
