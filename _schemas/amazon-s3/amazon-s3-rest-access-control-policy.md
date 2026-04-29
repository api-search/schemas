---
description: Contains the elements that set the ACL permissions for an object per grantee.
layout: schema
name: AccessControlPolicy
properties_list:
- description: ''
  name: AccessControlList
  type: object
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-rest-access-control-policy-schema.json
slug: amazon-s3-rest-access-control-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccessControlPolicy\",\n  \"type\": \"object\",\n  \"description\": \"Contains the elements that set the ACL permissions for an object per grantee.\",\n  \"properties\": {\n    \"AccessControlList\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-rest-access-control-policy-schema.json
tags:
- Archive
- AWS
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: AccessControlPolicy
---
