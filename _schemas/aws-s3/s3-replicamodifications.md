---
description: <p>A filter that you can specify for selection for modifications on replicas. Amazon S3 doesn't replicate replica modifications by default. In the latest version of replication configuration (when <code>Filter</code> is specified), you can specify this element and set the status to <code>Enabled</code> to replicate modifications on replicas. </p> <note> <p> If you don't specify the <code>Filter</code> element, Amazon S3 assumes that the replication configuration is the earlier version, V1. In the earlier version, this element is not allowed.</p> </note>
layout: schema
name: ReplicaModifications
properties_list:
- description: ''
  name: Status
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-replicamodifications-schema.json
slug: s3-replicamodifications
source_filename: s3-replicamodifications-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReplicaModifications\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {}\n  },\n  \"required\": [\n    \"Status\"\n  ],\n  \"description\": \"<p>A filter that you can specify for selection for modifications on replicas. Amazon S3 doesn't replicate replica modifications by default. In the latest version of replication configuration (when <code>Filter</code> is specified), you can specify this element and set the status to <code>Enabled</code> to replicate modifications on replicas. </p> <note> <p> If you don't specify the <code>Filter</code> element, Amazon S3 assumes that the replication configuration is the earlier version, V1. In the earlier version, this element is not allowed.</p> </note>\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-replicamodifications-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ReplicaModifications
---
