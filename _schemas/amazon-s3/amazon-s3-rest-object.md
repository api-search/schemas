---
description: An object consists of data and its descriptive metadata.
layout: schema
name: Object
properties_list:
- description: The name assigned to an object which identifies it in the bucket.
  name: Key
  type: string
- description: Date and time the object was last modified.
  name: LastModified
  type: string
- description: The entity tag is a hash of the object. The ETag reflects changes only to the contents of an object, not its metadata.
  name: ETag
  type: string
- description: Size in bytes of the object.
  name: Size
  type: integer
- description: The class of storage used to store the object.
  name: StorageClass
  type: string
- description: ''
  name: ChecksumAlgorithm
  type: array
- description: ''
  name: RestoreStatus
  type: object
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-rest-object-schema.json
slug: amazon-s3-rest-object
source_filename: amazon-s3-rest-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Object\",\n  \"type\": \"object\",\n  \"description\": \"An object consists of data and its descriptive metadata.\",\n  \"properties\": {\n    \"Key\": {\n      \"type\": \"string\",\n      \"description\": \"The name assigned to an object which identifies it in the bucket.\"\n    },\n    \"LastModified\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time the object was last modified.\"\n    },\n    \"ETag\": {\n      \"type\": \"string\",\n      \"description\": \"The entity tag is a hash of the object. The ETag reflects changes only to the contents of an object, not its metadata.\"\n    },\n    \"Size\": {\n      \"type\": \"integer\",\n      \"description\": \"Size in bytes of the object.\"\n    },\n    \"StorageClass\": {\n      \"type\": \"string\",\n      \"description\": \"The class of storage used to store the object.\"\n    },\n    \"ChecksumAlgorithm\": {\n   \
  \   \"type\": \"array\"\n    },\n    \"RestoreStatus\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-rest-object-schema.json
tags:
- Archive
- AWS
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: Object
---
