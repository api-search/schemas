---
description: Specifies the redirect behavior of all requests to a website endpoint of an Amazon S3 bucket.
layout: schema
name: RedirectAllRequestsTo
properties_list:
- description: ''
  name: HostName
  type: object
- description: ''
  name: Protocol
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-redirectallrequeststo-schema.json
slug: s3-redirectallrequeststo
source_filename: s3-redirectallrequeststo-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RedirectAllRequestsTo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HostName\": {},\n    \"Protocol\": {}\n  },\n  \"required\": [\n    \"HostName\"\n  ],\n  \"description\": \"Specifies the redirect behavior of all requests to a website endpoint of an Amazon S3 bucket.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-redirectallrequeststo-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: RedirectAllRequestsTo
---
