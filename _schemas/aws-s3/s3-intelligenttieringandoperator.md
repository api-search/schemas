---
description: A container for specifying S3 Intelligent-Tiering filters. The filters determine the subset of objects to which the rule applies.
layout: schema
name: IntelligentTieringAndOperator
properties_list:
- description: ''
  name: Prefix
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-intelligenttieringandoperator-schema.json
slug: s3-intelligenttieringandoperator
source_filename: s3-intelligenttieringandoperator-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IntelligentTieringAndOperator\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Prefix\": {},\n    \"Tags\": {}\n  },\n  \"description\": \"A container for specifying S3 Intelligent-Tiering filters. The filters determine the subset of objects to which the rule applies.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-intelligenttieringandoperator-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: IntelligentTieringAndOperator
---
