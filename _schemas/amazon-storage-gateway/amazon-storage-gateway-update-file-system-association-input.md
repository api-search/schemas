---
description: UpdateFileSystemAssociationInput schema from Amazon Storage Gateway API
layout: schema
name: UpdateFileSystemAssociationInput
properties_list:
- description: ''
  name: FileSystemAssociationARN
  type: object
- description: ''
  name: UserName
  type: object
- description: ''
  name: Password
  type: object
- description: ''
  name: AuditDestinationARN
  type: object
- description: ''
  name: CacheAttributes
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-update-file-system-association-input-schema.json
slug: amazon-storage-gateway-update-file-system-association-input
source_filename: amazon-storage-gateway-update-file-system-association-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-file-system-association-input-schema.json\",\n  \"title\": \"UpdateFileSystemAssociationInput\",\n  \"description\": \"UpdateFileSystemAssociationInput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileSystemAssociationARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileSystemAssociationARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the file system association that you want to update.\"\n        }\n      ]\n    },\n    \"UserName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainUserName\"\n        },\n        {\n          \"description\": \"The user name of the user credential that has permission to access\
  \ the root share D$ of the Amazon FSx file system. The user account must belong to the Amazon FSx delegated admin user group.\"\n        }\n      ]\n    },\n    \"Password\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainUserPassword\"\n        },\n        {\n          \"description\": \"The password of the user credential.\"\n        }\n      ]\n    },\n    \"AuditDestinationARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditDestinationARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the storage used for the audit logs.\"\n        }\n      ]\n    },\n    \"CacheAttributes\": {\n      \"$ref\": \"#/components/schemas/CacheAttributes\"\n    }\n  },\n  \"required\": [\n    \"FileSystemAssociationARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-file-system-association-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: UpdateFileSystemAssociationInput
---
