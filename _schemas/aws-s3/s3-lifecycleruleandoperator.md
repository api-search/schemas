---
description: This is used in a Lifecycle Rule Filter to apply a logical AND to two or more predicates. The Lifecycle Rule will apply to any object matching all of the predicates configured inside the And operator.
layout: schema
name: LifecycleRuleAndOperator
properties_list:
- description: ''
  name: Prefix
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: ObjectSizeGreaterThan
  type: object
- description: ''
  name: ObjectSizeLessThan
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-lifecycleruleandoperator-schema.json
slug: s3-lifecycleruleandoperator
source_filename: s3-lifecycleruleandoperator-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LifecycleRuleAndOperator\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Prefix\": {},\n    \"Tags\": {},\n    \"ObjectSizeGreaterThan\": {},\n    \"ObjectSizeLessThan\": {}\n  },\n  \"description\": \"This is used in a Lifecycle Rule Filter to apply a logical AND to two or more predicates. The Lifecycle Rule will apply to any object matching all of the predicates configured inside the And operator.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-lifecycleruleandoperator-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: LifecycleRuleAndOperator
---
