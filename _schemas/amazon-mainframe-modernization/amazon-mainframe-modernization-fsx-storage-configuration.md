---
description: Defines the storage configuration for an Amazon FSx file system.
layout: schema
name: FsxStorageConfiguration
properties_list:
- description: ''
  name: fileSystemId
  type: object
- description: ''
  name: mountPoint
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-fsx-storage-configuration-schema.json
slug: amazon-mainframe-modernization-fsx-storage-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-fsx-storage-configuration-schema.json\",\n  \"title\": \"FsxStorageConfiguration\",\n  \"description\": \"Defines the storage configuration for an Amazon FSx file system.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fileSystemId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String200\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"file-system-id\"\n          },\n          \"description\": \"The file system identifier.\"\n        }\n      ]\n    },\n    \"mountPoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String200\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mount-point\"\n          },\n          \"description\": \"The mount\
  \ point for the file system.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"fileSystemId\",\n    \"mountPoint\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-fsx-storage-configuration-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: FsxStorageConfiguration
---
