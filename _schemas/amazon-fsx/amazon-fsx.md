---
description: Represents an Amazon FSx file system with its associated configuration, state, and metadata.
layout: schema
name: Amazon FSx File System
properties_list:
- description: The unique identifier of the file system
  name: fileSystemId
  type: string
- description: The type of file system
  name: fileSystemType
  type: string
- description: The lifecycle status of the file system
  name: lifecycle
  type: string
- description: The storage capacity in GiB
  name: storageCapacity
  type: integer
- description: The storage type of the file system
  name: storageType
  type: string
- description: The ID of the VPC
  name: vpcId
  type: string
- description: The IDs of the subnets
  name: subnetIds
  type: array
- description: The DNS name for the file system
  name: dnsName
  type: string
- description: The AWS account that created the file system
  name: ownerId
  type: string
- description: The time the file system was created
  name: creationTime
  type: string
- description: Tags associated with the file system
  name: tags
  type: array
provider_name: Amazon FSx
provider_slug: amazon-fsx
schema_file: json-schema/amazon-fsx-schema.json
slug: amazon-fsx
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/amazon/fsx/filesystem.json\",\n  \"title\": \"Amazon FSx File System\",\n  \"description\": \"Represents an Amazon FSx file system with its associated configuration, state, and metadata.\",\n  \"type\": \"object\",\n  \"required\": [\"fileSystemId\", \"fileSystemType\", \"lifecycle\"],\n  \"properties\": {\n    \"fileSystemId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the file system\",\n      \"pattern\": \"^fs-[a-f0-9]{17}$\"\n    },\n    \"fileSystemType\": {\n      \"type\": \"string\",\n      \"enum\": [\"WINDOWS\", \"LUSTRE\", \"ONTAP\", \"OPENZFS\"],\n      \"description\": \"The type of file system\"\n    },\n    \"lifecycle\": {\n      \"type\": \"string\",\n      \"enum\": [\"AVAILABLE\", \"CREATING\", \"FAILED\", \"DELETING\", \"MISCONFIGURED\", \"UPDATING\"],\n      \"description\": \"The lifecycle status\
  \ of the file system\"\n    },\n    \"storageCapacity\": {\n      \"type\": \"integer\",\n      \"description\": \"The storage capacity in GiB\"\n    },\n    \"storageType\": {\n      \"type\": \"string\",\n      \"enum\": [\"SSD\", \"HDD\"],\n      \"description\": \"The storage type of the file system\"\n    },\n    \"vpcId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the VPC\"\n    },\n    \"subnetIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The IDs of the subnets\"\n    },\n    \"dnsName\": {\n      \"type\": \"string\",\n      \"description\": \"The DNS name for the file system\"\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS account that created the file system\"\n    },\n    \"creationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the file system was created\"\n    },\n    \"\
  tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags associated with the file system\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fsx/refs/heads/main/json-schema/amazon-fsx-schema.json
tags:
- AWS
- File Systems
- Lustre
- NetApp
- OpenZFS
- Storage
- Windows
title: Amazon FSx File System
---
