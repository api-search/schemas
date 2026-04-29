---
description: MountTarget schema from Amazon EFS Amazon Elastic File System (EFS) API
layout: schema
name: MountTarget
properties_list:
- description: System-assigned mount target ID.
  name: MountTargetId
  type: string
- description: The ID of the file system for which the mount target is intended.
  name: FileSystemId
  type: string
- description: The ID of the subnet.
  name: SubnetId
  type: string
- description: Lifecycle state of the mount target.
  name: LifeCycleState
  type: string
- description: Address at which the file system is mountable.
  name: IpAddress
  type: string
- description: The ID of the network interface.
  name: NetworkInterfaceId
  type: string
- description: The unique and consistent identifier of the Availability Zone.
  name: AvailabilityZoneId
  type: string
- description: The name of the Availability Zone.
  name: AvailabilityZoneName
  type: string
- description: The Virtual Private Cloud ID.
  name: VpcId
  type: string
provider_name: Amazon EFS
provider_slug: amazon-efs
schema_file: json-schema/efs-openapi-mount-target-schema.json
slug: efs-openapi-mount-target
source_filename: efs-openapi-mount-target-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-efs/refs/heads/main/json-schema/efs-openapi-mount-target-schema.json\",\n  \"title\": \"MountTarget\",\n  \"description\": \"MountTarget schema from Amazon EFS Amazon Elastic File System (EFS) API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MountTargetId\": {\n      \"type\": \"string\",\n      \"description\": \"System-assigned mount target ID.\"\n    },\n    \"FileSystemId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the file system for which the mount target is intended.\"\n    },\n    \"SubnetId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the subnet.\"\n    },\n    \"LifeCycleState\": {\n      \"type\": \"string\",\n      \"description\": \"Lifecycle state of the mount target.\"\n    },\n    \"IpAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Address at\
  \ which the file system is mountable.\"\n    },\n    \"NetworkInterfaceId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the network interface.\"\n    },\n    \"AvailabilityZoneId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique and consistent identifier of the Availability Zone.\"\n    },\n    \"AvailabilityZoneName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Availability Zone.\"\n    },\n    \"VpcId\": {\n      \"type\": \"string\",\n      \"description\": \"The Virtual Private Cloud ID.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-efs/refs/heads/main/json-schema/efs-openapi-mount-target-schema.json
tags:
- Amazon Web Services
- AWS
- EFS
- Elastic File System
- File Storage
- NFS
- Serverless
- Storage
title: MountTarget
---
