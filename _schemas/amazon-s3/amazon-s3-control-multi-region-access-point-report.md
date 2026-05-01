---
description: ''
layout: schema
name: MultiRegionAccessPointReport
properties_list:
- description: The name of the Multi-Region Access Point.
  name: Name
  type: string
- description: The alias for the Multi-Region Access Point.
  name: Alias
  type: string
- description: ''
  name: CreatedAt
  type: string
- description: ''
  name: Status
  type: string
- description: ''
  name: Regions
  type: array
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-control-multi-region-access-point-report-schema.json
slug: amazon-s3-control-multi-region-access-point-report
source_filename: amazon-s3-control-multi-region-access-point-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MultiRegionAccessPointReport\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Multi-Region Access Point.\"\n    },\n    \"Alias\": {\n      \"type\": \"string\",\n      \"description\": \"The alias for the Multi-Region Access Point.\"\n    },\n    \"CreatedAt\": {\n      \"type\": \"string\"\n    },\n    \"Status\": {\n      \"type\": \"string\"\n    },\n    \"Regions\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-control-multi-region-access-point-report-schema.json
tags:
- Archive
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: MultiRegionAccessPointReport
---
