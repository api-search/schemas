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
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: MetricsAndOperator
---
