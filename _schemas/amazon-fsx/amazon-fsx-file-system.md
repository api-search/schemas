---
description: An Amazon FSx fully managed file system (Lustre, Windows File Server, NetApp ONTAP, or OpenZFS).
layout: schema
name: FileSystem
properties_list:
- description: Unique identifier for the file system.
  name: FileSystemId
  type: string
- description: Type of the file system.
  name: FileSystemType
  type: string
- description: Current lifecycle state.
  name: Lifecycle
  type: string
- description: Storage capacity in GiB.
  name: StorageCapacity
  type: integer
- description: Type of storage media.
  name: StorageType
  type: string
- description: ID of the VPC containing the file system.
  name: VpcId
  type: string
- description: IDs of the subnets.
  name: SubnetIds
  type: array
- description: DNS name for the file system.
  name: DNSName
  type: string
- description: ID of the KMS key for encryption.
  name: KmsKeyId
  type: string
- description: ARN of the file system.
  name: ResourceARN
  type: string
- description: ''
  name: Tags
  type: array
- description: ''
  name: CreationTime
  type: string
- description: AWS account ID of the file system owner.
  name: OwnerId
  type: string
provider_name: Amazon FSx
provider_slug: amazon-fsx
schema_file: json-schema/amazon-fsx-file-system-schema.json
slug: amazon-fsx-file-system
source_filename: amazon-fsx-file-system-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fsx/refs/heads/main/json-schema/amazon-fsx-file-system-schema.json\",\n  \"title\": \"FileSystem\",\n  \"description\": \"An Amazon FSx fully managed file system (Lustre, Windows File Server, NetApp ONTAP, or OpenZFS).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileSystemId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the file system.\"\n    },\n    \"FileSystemType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"WINDOWS\",\n        \"LUSTRE\",\n        \"ONTAP\",\n        \"OPENZFS\"\n      ],\n      \"description\": \"Type of the file system.\"\n    },\n    \"Lifecycle\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"AVAILABLE\",\n        \"CREATING\",\n        \"FAILED\",\n        \"DELETING\",\n        \"MISCONFIGURED\",\n        \"UPDATING\",\n        \"\
  MISCONFIGURED_UNAVAILABLE\"\n      ],\n      \"description\": \"Current lifecycle state.\"\n    },\n    \"StorageCapacity\": {\n      \"type\": \"integer\",\n      \"description\": \"Storage capacity in GiB.\"\n    },\n    \"StorageType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SSD\",\n        \"HDD\"\n      ],\n      \"description\": \"Type of storage media.\"\n    },\n    \"VpcId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the VPC containing the file system.\"\n    },\n    \"SubnetIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"IDs of the subnets.\"\n    },\n    \"DNSName\": {\n      \"type\": \"string\",\n      \"description\": \"DNS name for the file system.\"\n    },\n    \"KmsKeyId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the KMS key for encryption.\"\n    },\n    \"ResourceARN\": {\n      \"type\": \"string\",\n      \"description\": \"\
  ARN of the file system.\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Tag\"\n      }\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"OwnerId\": {\n      \"type\": \"string\",\n      \"description\": \"AWS account ID of the file system owner.\"\n    }\n  },\n  \"required\": [\n    \"FileSystemType\",\n    \"StorageCapacity\",\n    \"SubnetIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fsx/refs/heads/main/json-schema/amazon-fsx-file-system-schema.json
tags:
- File Systems
- Lustre
- NetApp
- OpenZFS
- Storage
- Windows
title: FileSystem
---
