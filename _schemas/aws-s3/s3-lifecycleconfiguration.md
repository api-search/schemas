---
description: Container for lifecycle rules. You can add as many as 1000 rules.
layout: schema
name: LifecycleConfiguration
properties_list:
- description: ''
  name: Rules
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-lifecycleconfiguration-schema.json
slug: s3-lifecycleconfiguration
source_filename: s3-lifecycleconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LifecycleConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Rules\": {}\n  },\n  \"required\": [\n    \"Rules\"\n  ],\n  \"description\": \"Container for lifecycle rules. You can add as many as 1000 rules.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-lifecycleconfiguration-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: LifecycleConfiguration
---
