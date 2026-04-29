---
description: Represents a gateway's local disk.
layout: schema
name: Disk
properties_list:
- description: ''
  name: DiskId
  type: object
- description: ''
  name: DiskPath
  type: object
- description: ''
  name: DiskNode
  type: object
- description: ''
  name: DiskStatus
  type: object
- description: ''
  name: DiskSizeInBytes
  type: object
- description: ''
  name: DiskAllocationType
  type: object
- description: ''
  name: DiskAllocationResource
  type: object
- description: ''
  name: DiskAttributeList
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-disk-schema.json
slug: amazon-storage-gateway-disk
source_filename: amazon-storage-gateway-disk-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-disk-schema.json\",\n  \"title\": \"Disk\",\n  \"description\": \"Represents a gateway's local disk.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DiskId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DiskId\"\n        },\n        {\n          \"description\": \"The unique device ID or other distinguishing data that identifies a local disk.\"\n        }\n      ]\n    },\n    \"DiskPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"The path of a local disk in the gateway virtual machine (VM).\"\n        }\n      ]\n    },\n    \"DiskNode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n\
  \        {\n          \"description\": \"The device node of a local disk as assigned by the virtualization environment.\"\n        }\n      ]\n    },\n    \"DiskStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"A value that represents the status of a local disk.\"\n        }\n      ]\n    },\n    \"DiskSizeInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/long\"\n        },\n        {\n          \"description\": \"The local disk size in bytes.\"\n        }\n      ]\n    },\n    \"DiskAllocationType\": {\n      \"$ref\": \"#/components/schemas/DiskAllocationType\"\n    },\n    \"DiskAllocationResource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"The iSCSI qualified name (IQN) that is defined for a disk. This field is not included in the response if the local\
  \ disk is not defined as an iSCSI target. The format of this field is <i>targetIqn::LUNNumber::region-volumeId</i>.\"\n        }\n      ]\n    },\n    \"DiskAttributeList\": {\n      \"$ref\": \"#/components/schemas/DiskAttributeList\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-disk-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: Disk
---
