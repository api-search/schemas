---
description: FileSystem schema from Amazon EFS Amazon Elastic File System (EFS) API
layout: schema
name: FileSystem
properties_list:
- description: The ID of the file system.
  name: FileSystemId
  type: string
- description: The Amazon Resource Name (ARN) of the file system.
  name: FileSystemArn
  type: string
- description: The opaque string specified in the request.
  name: CreationToken
  type: string
- description: The AWS account that created the file system.
  name: OwnerId
  type: string
- description: The time that the file system was created.
  name: CreationTime
  type: string
- description: The lifecycle phase of the file system.
  name: LifeCycleState
  type: string
- description: The value of the Name tag if set.
  name: Name
  type: string
- description: The current number of mount targets that the file system has.
  name: NumberOfMountTargets
  type: integer
- description: The latest known metered size of data stored in the file system.
  name: SizeInBytes
  type: object
- description: The performance mode of the file system.
  name: PerformanceMode
  type: string
- description: A Boolean value that, if true, indicates that the file system is encrypted.
  name: Encrypted
  type: boolean
- description: The ID of the KMS key used for encryption.
  name: KmsKeyId
  type: string
- description: Displays the throughput mode for the file system.
  name: ThroughputMode
  type: string
- description: The amount of provisioned throughput, in MiB/s.
  name: ProvisionedThroughputInMibps
  type: number
- description: The tags associated with the file system.
  name: Tags
  type: array
provider_name: Amazon EFS
provider_slug: amazon-efs
schema_file: json-schema/efs-openapi-file-system-schema.json
slug: efs-openapi-file-system
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-efs/refs/heads/main/json-schema/efs-openapi-file-system-schema.json\",\n  \"title\": \"FileSystem\",\n  \"description\": \"FileSystem schema from Amazon EFS Amazon Elastic File System (EFS) API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileSystemId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the file system.\"\n    },\n    \"FileSystemArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the file system.\"\n    },\n    \"CreationToken\": {\n      \"type\": \"string\",\n      \"description\": \"The opaque string specified in the request.\"\n    },\n    \"OwnerId\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS account that created the file system.\"\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"The time that the file system was created.\"\n    },\n    \"LifeCycleState\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"creating\",\n        \"available\",\n        \"updating\",\n        \"deleting\",\n        \"deleted\",\n        \"error\"\n      ],\n      \"description\": \"The lifecycle phase of the file system.\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the Name tag if set.\"\n    },\n    \"NumberOfMountTargets\": {\n      \"type\": \"integer\",\n      \"description\": \"The current number of mount targets that the file system has.\"\n    },\n    \"SizeInBytes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Value\": {\n          \"type\": \"integer\",\n          \"description\": \"The latest known metered size of data stored in the file system, in bytes.\"\n        },\n        \"Timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\
  \n        },\n        \"ValueInIA\": {\n          \"type\": \"integer\"\n        },\n        \"ValueInStandard\": {\n          \"type\": \"integer\"\n        }\n      },\n      \"description\": \"The latest known metered size of data stored in the file system.\"\n    },\n    \"PerformanceMode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"generalPurpose\",\n        \"maxIO\"\n      ],\n      \"description\": \"The performance mode of the file system.\"\n    },\n    \"Encrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"A Boolean value that, if true, indicates that the file system is encrypted.\"\n    },\n    \"KmsKeyId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the KMS key used for encryption.\"\n    },\n    \"ThroughputMode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"bursting\",\n        \"provisioned\",\n        \"elastic\"\n      ],\n      \"description\": \"Displays the throughput mode for the file system.\"\
  \n    },\n    \"ProvisionedThroughputInMibps\": {\n      \"type\": \"number\",\n      \"description\": \"The amount of provisioned throughput, in MiB/s.\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Key\": {\n            \"type\": \"string\"\n          },\n          \"Value\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"description\": \"The tags associated with the file system.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-efs/refs/heads/main/json-schema/efs-openapi-file-system-schema.json
tags:
- Amazon Web Services
- AWS
- EFS
- Elastic File System
- File Storage
- NFS
- Serverless
- Storage
title: FileSystem
---
