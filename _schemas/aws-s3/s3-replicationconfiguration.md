---
description: A container for replication rules. You can add up to 1,000 rules. The maximum size of a replication configuration is 2 MB.
layout: schema
name: ReplicationConfiguration
properties_list:
- description: ''
  name: Role
  type: object
- description: ''
  name: Rules
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-replicationconfiguration-schema.json
slug: s3-replicationconfiguration
source_filename: s3-replicationconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReplicationConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Role\": {},\n    \"Rules\": {}\n  },\n  \"required\": [\n    \"Role\",\n    \"Rules\"\n  ],\n  \"description\": \"A container for replication rules. You can add up to 1,000 rules. The maximum size of a replication configuration is 2 MB.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-replicationconfiguration-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ReplicationConfiguration
---
