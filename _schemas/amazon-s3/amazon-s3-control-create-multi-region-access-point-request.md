---
description: ''
layout: schema
name: CreateMultiRegionAccessPointRequest
properties_list:
- description: An idempotency token used to identify the request.
  name: ClientToken
  type: string
- description: ''
  name: Details
  type: object
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-control-create-multi-region-access-point-request-schema.json
slug: amazon-s3-control-create-multi-region-access-point-request
source_filename: amazon-s3-control-create-multi-region-access-point-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateMultiRegionAccessPointRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClientToken\": {\n      \"type\": \"string\",\n      \"description\": \"An idempotency token used to identify the request.\"\n    },\n    \"Details\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-control-create-multi-region-access-point-request-schema.json
tags:
- Archive
- AWS
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: CreateMultiRegionAccessPointRequest
---
