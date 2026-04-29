---
description: Schema representing an Amazon Elastic File System, which provides a simple, serverless, set-and-forget elastic file system for use with AWS cloud services and on-premises resources.
layout: schema
name: Amazon EFS FileSystem
properties_list:
- description: The ID of the file system, assigned by Amazon EFS.
  name: FileSystemId
  type: string
- description: The Amazon Resource Name (ARN) of the EFS file system.
  name: FileSystemArn
  type: string
- description: The opaque string specified in the request to ensure idempotent creation.
  name: CreationToken
  type: string
- description: The AWS account that created the file system.
  name: OwnerId
  type: string
- description: The time that the file system was created, in seconds since epoch.
  name: CreationTime
  type: string
- description: The lifecycle phase of the file system.
  name: LifeCycleState
  type: string
- description: You can add tags to a file system, including a Name tag. If the file system has a Name tag, Amazon EFS returns the value in this field.
  name: Name
  type:
  - string
  - 'null'
- description: The current number of mount targets that the file system has.
  name: NumberOfMountTargets
  type: integer
- description: The latest known metered size (in bytes) of data stored in the file system.
  name: SizeInBytes
  type: object
- description: The performance mode of the file system.
  name: PerformanceMode
  type: string
- description: A Boolean value that, if true, indicates that the file system is encrypted.
  name: Encrypted
  type: boolean
- description: The ID of an AWS KMS key used to protect the encrypted file system.
  name: KmsKeyId
  type: string
- description: Displays the file system's throughput mode.
  name: ThroughputMode
  type: string
- description: The amount of provisioned throughput, measured in MiB/s, for the file system.
  name: ProvisionedThroughputInMibps
  type: number
- description: The unique and consistent identifier of the Availability Zone in which the file system is located.
  name: AvailabilityZoneId
  type:
  - string
  - 'null'
- description: Describes the AWS Availability Zone in which the file system is located.
  name: AvailabilityZoneName
  type:
  - string
  - 'null'
- description: The tags associated with the file system.
  name: Tags
  type: array
provider_name: Amazon EFS
provider_slug: amazon-efs
schema_file: json-schema/amazon-efs-filesystem-schema.json
slug: amazon-efs-filesystem
source_filename: amazon-efs-filesystem-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.apis.io/schemas/amazon-efs-filesystem.json\",\n  \"title\": \"Amazon EFS FileSystem\",\n  \"description\": \"Schema representing an Amazon Elastic File System, which provides a simple, serverless, set-and-forget elastic file system for use with AWS cloud services and on-premises resources.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"CreationToken\"\n  ],\n  \"properties\": {\n    \"FileSystemId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the file system, assigned by Amazon EFS.\",\n      \"pattern\": \"^fs-[a-f0-9]+$\"\n    },\n    \"FileSystemArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the EFS file system.\",\n      \"pattern\": \"^arn:aws[a-zA-Z-]*:elasticfilesystem:[a-z0-9-]+:[0-9]{12}:file-system/fs-.+$\"\n    },\n    \"CreationToken\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The opaque string specified in the request to ensure idempotent creation.\",\n      \"minLength\": 1,\n      \"maxLength\": 64\n    },\n    \"OwnerId\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS account that created the file system.\",\n      \"pattern\": \"^[0-9]{12}$\"\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time that the file system was created, in seconds since epoch.\"\n    },\n    \"LifeCycleState\": {\n      \"type\": \"string\",\n      \"description\": \"The lifecycle phase of the file system.\",\n      \"enum\": [\n        \"creating\",\n        \"available\",\n        \"updating\",\n        \"deleting\",\n        \"deleted\",\n        \"error\"\n      ]\n    },\n    \"Name\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"You can add tags to a file system, including a Name tag. If the file system has a Name tag, Amazon EFS returns the value in\
  \ this field.\",\n      \"maxLength\": 256\n    },\n    \"NumberOfMountTargets\": {\n      \"type\": \"integer\",\n      \"description\": \"The current number of mount targets that the file system has.\",\n      \"minimum\": 0\n    },\n    \"SizeInBytes\": {\n      \"type\": \"object\",\n      \"description\": \"The latest known metered size (in bytes) of data stored in the file system.\",\n      \"properties\": {\n        \"Value\": {\n          \"type\": \"integer\",\n          \"description\": \"The latest known metered size (in bytes) of data stored in the file system.\",\n          \"minimum\": 0\n        },\n        \"Timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The time at which the size of data was determined.\"\n        },\n        \"ValueInIA\": {\n          \"type\": \"integer\",\n          \"description\": \"The latest known metered size (in bytes) of data stored in the Infrequent Access storage class.\"\
  ,\n          \"minimum\": 0\n        },\n        \"ValueInStandard\": {\n          \"type\": \"integer\",\n          \"description\": \"The latest known metered size (in bytes) of data stored in the Standard storage class.\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"PerformanceMode\": {\n      \"type\": \"string\",\n      \"description\": \"The performance mode of the file system.\",\n      \"enum\": [\n        \"generalPurpose\",\n        \"maxIO\"\n      ],\n      \"default\": \"generalPurpose\"\n    },\n    \"Encrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"A Boolean value that, if true, indicates that the file system is encrypted.\",\n      \"default\": false\n    },\n    \"KmsKeyId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of an AWS KMS key used to protect the encrypted file system.\"\n    },\n    \"ThroughputMode\": {\n      \"type\": \"string\",\n      \"description\": \"Displays the file system's throughput mode.\"\
  ,\n      \"enum\": [\n        \"bursting\",\n        \"provisioned\",\n        \"elastic\"\n      ],\n      \"default\": \"bursting\"\n    },\n    \"ProvisionedThroughputInMibps\": {\n      \"type\": \"number\",\n      \"description\": \"The amount of provisioned throughput, measured in MiB/s, for the file system.\",\n      \"minimum\": 1,\n      \"maximum\": 3414\n    },\n    \"AvailabilityZoneId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The unique and consistent identifier of the Availability Zone in which the file system is located.\"\n    },\n    \"AvailabilityZoneName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Describes the AWS Availability Zone in which the file system is located.\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"description\": \"The tags associated with the file system.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\n          \"Key\",\n          \"Value\"\n\
  \        ],\n        \"properties\": {\n          \"Key\": {\n            \"type\": \"string\",\n            \"description\": \"The tag key.\",\n            \"minLength\": 1,\n            \"maxLength\": 128\n          },\n          \"Value\": {\n            \"type\": \"string\",\n            \"description\": \"The value of the tag key.\",\n            \"minLength\": 0,\n            \"maxLength\": 256\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-efs/refs/heads/main/json-schema/amazon-efs-filesystem-schema.json
tags:
- Amazon Web Services
- AWS
- EFS
- Elastic File System
- File Storage
- NFS
- Serverless
- Storage
title: Amazon EFS FileSystem
---
