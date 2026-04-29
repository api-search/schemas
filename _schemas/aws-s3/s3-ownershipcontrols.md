---
description: The container element for a bucket's ownership controls.
layout: schema
name: OwnershipControls
properties_list:
- description: ''
  name: Rules
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-ownershipcontrols-schema.json
slug: s3-ownershipcontrols
source_filename: s3-ownershipcontrols-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OwnershipControls\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Rules\": {}\n  },\n  \"required\": [\n    \"Rules\"\n  ],\n  \"description\": \"The container element for a bucket's ownership controls.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-ownershipcontrols-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: OwnershipControls
---
