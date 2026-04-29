---
description: Defines the storage configuration for a runtime environment.
layout: schema
name: StorageConfiguration
properties_list:
- description: ''
  name: efs
  type: object
- description: ''
  name: fsx
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-storage-configuration-schema.json
slug: amazon-mainframe-modernization-storage-configuration
source_filename: amazon-mainframe-modernization-storage-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-storage-configuration-schema.json\",\n  \"title\": \"StorageConfiguration\",\n  \"description\": \"Defines the storage configuration for a runtime environment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"efs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EfsStorageConfiguration\"\n        },\n        {\n          \"description\": \"Defines the storage configuration for an Amazon EFS file system.\"\n        }\n      ]\n    },\n    \"fsx\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FsxStorageConfiguration\"\n        },\n        {\n          \"description\": \"Defines the storage configuration for an Amazon FSx file system.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-storage-configuration-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: StorageConfiguration
---
