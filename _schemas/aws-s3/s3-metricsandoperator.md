---
description: A conjunction (logical AND) of predicates, which is used in evaluating a metrics filter. The operator must have at least two predicates, and an object must match all of the predicates in order for the filter to apply.
layout: schema
name: MetricsAndOperator
properties_list:
- description: ''
  name: Prefix
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: AccessPointArn
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-metricsandoperator-schema.json
slug: s3-metricsandoperator
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricsAndOperator\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Prefix\": {},\n    \"Tags\": {},\n    \"AccessPointArn\": {}\n  },\n  \"description\": \"A conjunction (logical AND) of predicates, which is used in evaluating a metrics filter. The operator must have at least two predicates, and an object must match all of the predicates in order for the filter to apply.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-metricsandoperator-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: MetricsAndOperator
---
