---
description: Describes Network File System (NFS) file share default values. Files and folders stored as Amazon S3 objects in S3 buckets don't, by default, have Unix file permissions assigned to them. Upon discovery in an S3 bucket by Storage Gateway, the S3 objects that represent files and folders are assigned these default Unix permissions. This operation is only supported for S3 File Gateways.
layout: schema
name: NFSFileShareDefaults
properties_list:
- description: ''
  name: FileMode
  type: object
- description: ''
  name: DirectoryMode
  type: object
- description: ''
  name: GroupId
  type: object
- description: ''
  name: OwnerId
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-nfs-file-share-defaults-schema.json
slug: amazon-storage-gateway-nfs-file-share-defaults
source_filename: amazon-storage-gateway-nfs-file-share-defaults-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-nfs-file-share-defaults-schema.json\",\n  \"title\": \"NFSFileShareDefaults\",\n  \"description\": \"Describes Network File System (NFS) file share default values. Files and folders stored as Amazon S3 objects in S3 buckets don't, by default, have Unix file permissions assigned to them. Upon discovery in an S3 bucket by Storage Gateway, the S3 objects that represent files and folders are assigned these default Unix permissions. This operation is only supported for S3 File Gateways.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionMode\"\n        },\n        {\n          \"description\": \"The Unix file mode in the form \\\"nnnn\\\". For example, <code>0666</code> represents\
  \ the default file mode inside the file share. The default value is <code>0666</code>.\"\n        }\n      ]\n    },\n    \"DirectoryMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionMode\"\n        },\n        {\n          \"description\": \"The Unix directory mode in the form \\\"nnnn\\\". For example, <code>0666</code> represents the default access mode for all directories inside the file share. The default value is <code>0777</code>.\"\n        }\n      ]\n    },\n    \"GroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionId\"\n        },\n        {\n          \"description\": \"The default group ID for the file share (unless the files have another group ID specified). The default value is <code>nfsnobody</code>.\"\n        }\n      ]\n    },\n    \"OwnerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionId\"\n        },\n        {\n          \"description\"\
  : \"The default owner ID for files in the file share (unless the files have another owner ID specified). The default value is <code>nfsnobody</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-nfs-file-share-defaults-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: NFSFileShareDefaults
---
