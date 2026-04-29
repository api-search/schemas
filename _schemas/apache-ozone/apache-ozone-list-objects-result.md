---
description: ListObjectsResult schema from Apache Ozone
layout: schema
name: ListObjectsResult
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: prefix
  type: string
- description: ''
  name: maxKeys
  type: integer
- description: ''
  name: isTruncated
  type: boolean
- description: ''
  name: nextContinuationToken
  type: string
- description: ''
  name: contents
  type: array
provider_name: Apache Ozone
provider_slug: apache-ozone
schema_file: json-schema/apache-ozone-list-objects-result-schema.json
slug: apache-ozone-list-objects-result
source_filename: apache-ozone-list-objects-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ozone/refs/heads/main/json-schema/apache-ozone-list-objects-result-schema.json\",\n  \"title\": \"ListObjectsResult\",\n  \"description\": \"ListObjectsResult schema from Apache Ozone\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"my-bucket\"\n    },\n    \"prefix\": {\n      \"type\": \"string\",\n      \"example\": \"data/\"\n    },\n    \"maxKeys\": {\n      \"type\": \"integer\",\n      \"example\": 1000\n    },\n    \"isTruncated\": {\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"nextContinuationToken\": {\n      \"type\": \"string\"\n    },\n    \"contents\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ozone/refs/heads/main/json-schema/apache-ozone-list-objects-result-schema.json
tags:
- Distributed Storage
- Hadoop
- Object Storage
- S3-Compatible
- Apache
- Open Source
title: ListObjectsResult
---
