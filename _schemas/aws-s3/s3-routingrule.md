---
description: Specifies the redirect behavior and when a redirect is applied. For more information about routing rules, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/how-to-page-redirect.html#advanced-conditional-redirects">Configuring advanced conditional redirects</a> in the <i>Amazon S3 User Guide</i>.
layout: schema
name: RoutingRule
properties_list:
- description: ''
  name: Condition
  type: object
- description: ''
  name: Redirect
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-routingrule-schema.json
slug: s3-routingrule
source_filename: s3-routingrule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RoutingRule\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Condition\": {},\n    \"Redirect\": {}\n  },\n  \"required\": [\n    \"Redirect\"\n  ],\n  \"description\": \"Specifies the redirect behavior and when a redirect is applied. For more information about routing rules, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/how-to-page-redirect.html#advanced-conditional-redirects\\\">Configuring advanced conditional redirects</a> in the <i>Amazon S3 User Guide</i>.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-routingrule-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: RoutingRule
---
