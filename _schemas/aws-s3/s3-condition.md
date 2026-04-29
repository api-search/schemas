---
description: A container for describing a condition that must be met for the specified redirect to apply. For example, 1. If request is for pages in the <code>/docs</code> folder, redirect to the <code>/documents</code> folder. 2. If request results in HTTP error 4xx, redirect request to another host where you might process the error.
layout: schema
name: Condition
properties_list:
- description: ''
  name: HttpErrorCodeReturnedEquals
  type: object
- description: ''
  name: KeyPrefixEquals
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-condition-schema.json
slug: s3-condition
source_filename: s3-condition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Condition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HttpErrorCodeReturnedEquals\": {},\n    \"KeyPrefixEquals\": {}\n  },\n  \"description\": \"A container for describing a condition that must be met for the specified redirect to apply. For example, 1. If request is for pages in the <code>/docs</code> folder, redirect to the <code>/documents</code> folder. 2. If request results in HTTP error 4xx, redirect request to another host where you might process the error.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-condition-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: Condition
---
