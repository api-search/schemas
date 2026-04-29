---
description: A value that sets the access control list (ACL) permission for objects in the S3 bucket that an S3 File Gateway puts objects into. The default value is <code>private</code>.
layout: schema
name: ObjectACL
properties_list: []
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-object-acl-schema.json
slug: amazon-storage-gateway-object-acl
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-object-acl-schema.json\",\n  \"title\": \"ObjectACL\",\n  \"description\": \"A value that sets the access control list (ACL) permission for objects in the S3 bucket that an S3 File Gateway puts objects into. The default value is <code>private</code>.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"private\",\n    \"public-read\",\n    \"public-read-write\",\n    \"authenticated-read\",\n    \"bucket-owner-read\",\n    \"bucket-owner-full-control\",\n    \"aws-exec-read\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-object-acl-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: ObjectACL
---
