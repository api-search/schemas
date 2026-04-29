---
description: Container for grant information.
layout: schema
name: Grant
properties_list:
- description: The person being granted permissions.
  name: Grantee
  type: object
- description: Specifies the permission given to the grantee.
  name: Permission
  type: string
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-rest-grant-schema.json
slug: amazon-s3-rest-grant
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Grant\",\n  \"type\": \"object\",\n  \"description\": \"Container for grant information.\",\n  \"properties\": {\n    \"Grantee\": {\n      \"type\": \"object\",\n      \"description\": \"The person being granted permissions.\"\n    },\n    \"Permission\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the permission given to the grantee.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-rest-grant-schema.json
tags:
- Archive
- AWS
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: Grant
---
