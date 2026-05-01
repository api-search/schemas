---
description: Contains the elements that set the ACL permissions for an object per grantee.
layout: schema
name: AccessControlPolicy
properties_list:
- description: ''
  name: Grants
  type: object
- description: ''
  name: Owner
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-accesscontrolpolicy-schema.json
slug: s3-accesscontrolpolicy
source_filename: s3-accesscontrolpolicy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccessControlPolicy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Grants\": {},\n    \"Owner\": {}\n  },\n  \"description\": \"Contains the elements that set the ACL permissions for an object per grantee.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-accesscontrolpolicy-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: AccessControlPolicy
---
