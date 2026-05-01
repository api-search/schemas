---
description: Gets the summary returned by <code>ListFileSystemAssociation</code>, which is a summary of a created file system association.
layout: schema
name: FileSystemAssociationSummary
properties_list:
- description: ''
  name: FileSystemAssociationId
  type: object
- description: ''
  name: FileSystemAssociationARN
  type: object
- description: ''
  name: FileSystemAssociationStatus
  type: object
- description: ''
  name: GatewayARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-file-system-association-summary-schema.json
slug: amazon-storage-gateway-file-system-association-summary
source_filename: amazon-storage-gateway-file-system-association-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-file-system-association-summary-schema.json\",\n  \"title\": \"FileSystemAssociationSummary\",\n  \"description\": \"Gets the summary returned by <code>ListFileSystemAssociation</code>, which is a summary of a created file system association.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileSystemAssociationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileSystemAssociationId\"\n        },\n        {\n          \"description\": \"The ID of the file system association.\"\n        }\n      ]\n    },\n    \"FileSystemAssociationARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileSystemAssociationARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the file\
  \ system association.\"\n        }\n      ]\n    },\n    \"FileSystemAssociationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileSystemAssociationStatus\"\n        },\n        {\n          \"description\": \"The status of the file share. Valid Values: <code>AVAILABLE</code> | <code>CREATING</code> | <code>DELETING</code> | <code>FORCE_DELETING</code> | <code>UPDATING</code> | <code>ERROR</code> \"\n        }\n      ]\n    },\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-file-system-association-summary-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: FileSystemAssociationSummary
---
