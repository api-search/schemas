---
description: CreateTrailResponse schema
layout: schema
name: CreateTrailResponse
properties_list:
- description: ''
  name: Name
  type: string
- description: ''
  name: S3BucketName
  type: string
- description: ''
  name: TrailARN
  type: string
- description: ''
  name: IsMultiRegionTrail
  type: boolean
- description: ''
  name: LogFileValidationEnabled
  type: boolean
provider_name: Amazon CloudTrail
provider_slug: amazon-cloudtrail
schema_file: json-schema/cloudtrail-create-trail-response-schema.json
slug: cloudtrail-create-trail-response
source_filename: cloudtrail-create-trail-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudtrail/refs/heads/main/json-schema/cloudtrail-create-trail-response-schema.json\",\n  \"title\": \"CreateTrailResponse\",\n  \"description\": \"CreateTrailResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\"\n    },\n    \"S3BucketName\": {\n      \"type\": \"string\"\n    },\n    \"TrailARN\": {\n      \"type\": \"string\"\n    },\n    \"IsMultiRegionTrail\": {\n      \"type\": \"boolean\"\n    },\n    \"LogFileValidationEnabled\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudtrail/refs/heads/main/json-schema/cloudtrail-create-trail-response-schema.json
tags:
- AWS
- CloudTrail
- Audit
- Compliance
- Governance
- Security
title: CreateTrailResponse
---
