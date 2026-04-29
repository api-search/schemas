---
description: A conjunction (logical AND) of predicates, which is used in evaluating a metrics filter. The operator must have at least two predicates in any combination, and an object must match all of the predicates for the filter to apply.
layout: schema
name: AnalyticsAndOperator
properties_list:
- description: ''
  name: Prefix
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-analyticsandoperator-schema.json
slug: s3-analyticsandoperator
source_filename: s3-analyticsandoperator-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AnalyticsAndOperator\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Prefix\": {},\n    \"Tags\": {}\n  },\n  \"description\": \"A conjunction (logical AND) of predicates, which is used in evaluating a metrics filter. The operator must have at least two predicates in any combination, and an object must match all of the predicates for the filter to apply.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-analyticsandoperator-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: AnalyticsAndOperator
---
