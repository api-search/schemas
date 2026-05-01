---
description: Container for the objects to delete.
layout: schema
name: Delete
properties_list:
- description: Container element that describes the delete request for an object.
  name: Object
  type: array
- description: Element to enable quiet mode for the request. When added, it must be set to true.
  name: Quiet
  type: boolean
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-rest-delete-schema.json
slug: amazon-s3-rest-delete
source_filename: amazon-s3-rest-delete-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Delete\",\n  \"type\": \"object\",\n  \"description\": \"Container for the objects to delete.\",\n  \"properties\": {\n    \"Object\": {\n      \"type\": \"array\",\n      \"description\": \"Container element that describes the delete request for an object.\"\n    },\n    \"Quiet\": {\n      \"type\": \"boolean\",\n      \"description\": \"Element to enable quiet mode for the request. When added, it must be set to true.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-rest-delete-schema.json
tags:
- Archive
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: Delete
---
