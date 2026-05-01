---
description: A storage virtual machine (SVM) in an Amazon FSx for NetApp ONTAP file system.
layout: schema
name: StorageVirtualMachine
properties_list:
- description: Active Directory configuration for the SVM.
  name: ActiveDirectoryConfiguration
  type: object
- description: ''
  name: CreationTime
  type: string
- description: Endpoints for accessing the SVM via different protocols.
  name: Endpoints
  type: object
- description: ''
  name: FileSystemId
  type: string
- description: ''
  name: Lifecycle
  type: string
- description: Name of the SVM.
  name: Name
  type: string
- description: ''
  name: ResourceARN
  type: string
- description: ''
  name: StorageVirtualMachineId
  type: string
- description: ''
  name: Subtype
  type: string
- description: ''
  name: Tags
  type: array
- description: ''
  name: UUID
  type: string
provider_name: Amazon FSx
provider_slug: amazon-fsx
schema_file: json-schema/amazon-fsx-storage-virtual-machine-schema.json
slug: amazon-fsx-storage-virtual-machine
source_filename: amazon-fsx-storage-virtual-machine-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fsx/refs/heads/main/json-schema/amazon-fsx-storage-virtual-machine-schema.json\",\n  \"title\": \"StorageVirtualMachine\",\n  \"description\": \"A storage virtual machine (SVM) in an Amazon FSx for NetApp ONTAP file system.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActiveDirectoryConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"Active Directory configuration for the SVM.\"\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"Endpoints\": {\n      \"type\": \"object\",\n      \"description\": \"Endpoints for accessing the SVM via different protocols.\"\n    },\n    \"FileSystemId\": {\n      \"type\": \"string\"\n    },\n    \"Lifecycle\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREATED\",\n        \"CREATING\",\n        \"\
  DELETING\",\n        \"FAILED\",\n        \"MISCONFIGURED\",\n        \"PENDING\"\n      ]\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the SVM.\"\n    },\n    \"ResourceARN\": {\n      \"type\": \"string\"\n    },\n    \"StorageVirtualMachineId\": {\n      \"type\": \"string\"\n    },\n    \"Subtype\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"DEFAULT\",\n        \"DP_DESTINATION\",\n        \"SYNC_DESTINATION\",\n        \"SYNC_SOURCE\"\n      ]\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"UUID\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"FileSystemId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fsx/refs/heads/main/json-schema/amazon-fsx-storage-virtual-machine-schema.json
tags:
- File Systems
- Lustre
- NetApp
- OpenZFS
- Storage
- Windows
title: StorageVirtualMachine
---
