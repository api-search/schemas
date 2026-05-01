---
description: Optional configuration to replicate existing source bucket objects. For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/replication-what-is-isnot-replicated.html#existing-object-replication">Replicating Existing Objects</a> in the <i>Amazon S3 User Guide</i>.
layout: schema
name: ExistingObjectReplication
properties_list:
- description: ''
  name: Status
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-existingobjectreplication-schema.json
slug: s3-existingobjectreplication
source_filename: s3-existingobjectreplication-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExistingObjectReplication\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {}\n  },\n  \"required\": [\n    \"Status\"\n  ],\n  \"description\": \"Optional configuration to replicate existing source bucket objects. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/replication-what-is-isnot-replicated.html#existing-object-replication\\\">Replicating Existing Objects</a> in the <i>Amazon S3 User Guide</i>. \"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-existingobjectreplication-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: ExistingObjectReplication
---
