---
description: A container specifying S3 Replication Time Control (S3 RTC) related information, including whether S3 RTC is enabled and the time when all objects and operations on objects must be replicated. Must be specified together with a <code>Metrics</code> block.
layout: schema
name: ReplicationTime
properties_list:
- description: ''
  name: Status
  type: object
- description: ''
  name: Time
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-replicationtime-schema.json
slug: s3-replicationtime
source_filename: s3-replicationtime-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReplicationTime\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {},\n    \"Time\": {}\n  },\n  \"required\": [\n    \"Status\",\n    \"Time\"\n  ],\n  \"description\": \" A container specifying S3 Replication Time Control (S3 RTC) related information, including whether S3 RTC is enabled and the time when all objects and operations on objects must be replicated. Must be specified together with a <code>Metrics</code> block. \"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-replicationtime-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: ReplicationTime
---
