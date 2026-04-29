---
description: Container for the owner's display name and ID.
layout: schema
name: Owner
properties_list:
- description: Container for the display name of the owner.
  name: DisplayName
  type: string
- description: Container for the ID of the owner.
  name: ID
  type: string
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-rest-owner-schema.json
slug: amazon-s3-rest-owner
source_filename: amazon-s3-rest-owner-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Owner\",\n  \"type\": \"object\",\n  \"description\": \"Container for the owner's display name and ID.\",\n  \"properties\": {\n    \"DisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"Container for the display name of the owner.\"\n    },\n    \"ID\": {\n      \"type\": \"string\",\n      \"description\": \"Container for the ID of the owner.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-rest-owner-schema.json
tags:
- Archive
- AWS
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: Owner
---
