---
description: Specifies website configuration parameters for an Amazon S3 bucket.
layout: schema
name: WebsiteConfiguration
properties_list:
- description: ''
  name: ErrorDocument
  type: object
- description: ''
  name: IndexDocument
  type: object
- description: ''
  name: RedirectAllRequestsTo
  type: object
- description: ''
  name: RoutingRules
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-websiteconfiguration-schema.json
slug: s3-websiteconfiguration
source_filename: s3-websiteconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WebsiteConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ErrorDocument\": {},\n    \"IndexDocument\": {},\n    \"RedirectAllRequestsTo\": {},\n    \"RoutingRules\": {}\n  },\n  \"description\": \"Specifies website configuration parameters for an Amazon S3 bucket.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-websiteconfiguration-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: WebsiteConfiguration
---
