---
description: The <code>Filter</code> is used to identify objects that the S3 Intelligent-Tiering configuration applies to.
layout: schema
name: IntelligentTieringFilter
properties_list:
- description: ''
  name: Prefix
  type: object
- description: A container of a key value name pair.
  name: Tag
  type: object
- description: ''
  name: And
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-intelligenttieringfilter-schema.json
slug: s3-intelligenttieringfilter
source_filename: s3-intelligenttieringfilter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IntelligentTieringFilter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Prefix\": {},\n    \"Tag\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Key\": {},\n        \"Value\": {}\n      },\n      \"required\": [\n        \"Key\",\n        \"Value\"\n      ],\n      \"description\": \"A container of a key value name pair.\"\n    },\n    \"And\": {}\n  },\n  \"description\": \"The <code>Filter</code> is used to identify objects that the S3 Intelligent-Tiering configuration applies to.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-intelligenttieringfilter-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: IntelligentTieringFilter
---
