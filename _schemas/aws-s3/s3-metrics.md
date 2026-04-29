---
description: A container specifying replication metrics-related settings enabling replication metrics and events.
layout: schema
name: Metrics
properties_list:
- description: ''
  name: Status
  type: object
- description: ''
  name: EventThreshold
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-metrics-schema.json
slug: s3-metrics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Metrics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {},\n    \"EventThreshold\": {}\n  },\n  \"required\": [\n    \"Status\"\n  ],\n  \"description\": \" A container specifying replication metrics-related settings enabling replication metrics and events.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-metrics-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: Metrics
---
