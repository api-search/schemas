---
description: The <code>Filter</code> is used to identify objects that a Lifecycle Rule applies to. A <code>Filter</code> must have exactly one of <code>Prefix</code>, <code>Tag</code>, or <code>And</code> specified.
layout: schema
name: LifecycleRuleFilter
properties_list:
- description: ''
  name: Prefix
  type: object
- description: ''
  name: Tag
  type: object
- description: ''
  name: ObjectSizeGreaterThan
  type: object
- description: ''
  name: ObjectSizeLessThan
  type: object
- description: This is used in a Lifecycle Rule Filter to apply a logical AND to two or more predicates. The Lifecycle Rule will apply to any object matching all of the predicates configured inside the And operator.
  name: And
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-lifecyclerulefilter-schema.json
slug: s3-lifecyclerulefilter
source_filename: s3-lifecyclerulefilter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LifecycleRuleFilter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Prefix\": {},\n    \"Tag\": {},\n    \"ObjectSizeGreaterThan\": {},\n    \"ObjectSizeLessThan\": {},\n    \"And\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Prefix\": {},\n        \"Tags\": {},\n        \"ObjectSizeGreaterThan\": {},\n        \"ObjectSizeLessThan\": {}\n      },\n      \"description\": \"This is used in a Lifecycle Rule Filter to apply a logical AND to two or more predicates. The Lifecycle Rule will apply to any object matching all of the predicates configured inside the And operator.\"\n    }\n  },\n  \"description\": \"The <code>Filter</code> is used to identify objects that a Lifecycle Rule applies to. A <code>Filter</code> must have exactly one of <code>Prefix</code>, <code>Tag</code>, or <code>And</code> specified.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-lifecyclerulefilter-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: LifecycleRuleFilter
---
