---
description: DisassociateFileSystemInput schema from Amazon Storage Gateway API
layout: schema
name: DisassociateFileSystemInput
properties_list:
- description: ''
  name: FileSystemAssociationARN
  type: object
- description: ''
  name: ForceDelete
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-disassociate-file-system-input-schema.json
slug: amazon-storage-gateway-disassociate-file-system-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-disassociate-file-system-input-schema.json\",\n  \"title\": \"DisassociateFileSystemInput\",\n  \"description\": \"DisassociateFileSystemInput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileSystemAssociationARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileSystemAssociationARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the file system association to be deleted.\"\n        }\n      ]\n    },\n    \"ForceDelete\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/boolean\"\n        },\n        {\n          \"description\": \"If this value is set to true, the operation disassociates an Amazon FSx file system immediately.\
  \ It ends all data uploads to the file system, and the file system association enters the <code>FORCE_DELETING</code> status. If this value is set to false, the Amazon FSx file system does not disassociate until all data is uploaded.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FileSystemAssociationARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-disassociate-file-system-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DisassociateFileSystemInput
---
