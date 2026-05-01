---
description: Schema for a Storage Transfer Service transfer job configuration, used to define data transfer operations between storage systems.
layout: schema
name: Google Cloud Storage Transfer Job
properties_list:
- description: A unique name for the transfer job, auto-generated if not provided
  name: name
  type: string
- description: A description provided by the user for the transfer job
  name: description
  type: string
- description: The ID of the Google Cloud project that owns the job
  name: projectId
  type: string
- description: Transfer specification describing source and destination
  name: transferSpec
  type: object
- description: Schedule for the transfer job
  name: schedule
  type: object
- description: Status of the transfer job
  name: status
  type: string
- description: Timestamp when the job was created
  name: creationTime
  type: string
- description: Timestamp when the job was last modified
  name: lastModificationTime
  type: string
provider_name: Google Cloud Transfer Service
provider_slug: google-cloud-transfer-service
schema_file: json-schema/google-cloud-transfer-service-job-schema.json
slug: google-cloud-transfer-service-job
source_filename: google-cloud-transfer-service-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://cloud.google.com/schemas/storagetransfer/transfer-job.json\",\n  \"title\": \"Google Cloud Storage Transfer Job\",\n  \"description\": \"Schema for a Storage Transfer Service transfer job configuration, used to define data transfer operations between storage systems.\",\n  \"type\": \"object\",\n  \"required\": [\"projectId\", \"transferSpec\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"A unique name for the transfer job, auto-generated if not provided\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description provided by the user for the transfer job\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the Google Cloud project that owns the job\"\n    },\n    \"transferSpec\": {\n      \"$ref\": \"#/$defs/TransferSpec\",\n      \"description\": \"\
  Transfer specification describing source and destination\"\n    },\n    \"schedule\": {\n      \"$ref\": \"#/$defs/Schedule\",\n      \"description\": \"Schedule for the transfer job\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the transfer job\",\n      \"enum\": [\"STATUS_UNSPECIFIED\", \"ENABLED\", \"DISABLED\", \"DELETED\"]\n    },\n    \"creationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the job was created\"\n    },\n    \"lastModificationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the job was last modified\"\n    }\n  },\n  \"$defs\": {\n    \"TransferSpec\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for running a transfer between source and destination\",\n      \"properties\": {\n        \"gcsDataSink\": {\n          \"$ref\": \"#/$defs/GcsData\",\n          \"\
  description\": \"Google Cloud Storage destination bucket\"\n        },\n        \"gcsDataSource\": {\n          \"$ref\": \"#/$defs/GcsData\",\n          \"description\": \"Google Cloud Storage source bucket\"\n        },\n        \"awsS3DataSource\": {\n          \"$ref\": \"#/$defs/AwsS3Data\",\n          \"description\": \"Amazon S3 source bucket\"\n        },\n        \"azureBlobStorageDataSource\": {\n          \"$ref\": \"#/$defs/AzureBlobStorageData\",\n          \"description\": \"Azure Blob Storage source container\"\n        },\n        \"objectConditions\": {\n          \"type\": \"object\",\n          \"description\": \"Conditions to determine which objects are transferred\",\n          \"properties\": {\n            \"includePrefixes\": {\n              \"type\": \"array\",\n              \"items\": { \"type\": \"string\" }\n            },\n            \"excludePrefixes\": {\n              \"type\": \"array\",\n              \"items\": { \"type\": \"string\" }\n          \
  \  }\n          }\n        },\n        \"transferOptions\": {\n          \"type\": \"object\",\n          \"description\": \"Options controlling transfer behavior\",\n          \"properties\": {\n            \"overwriteObjectsAlreadyExistingInSink\": {\n              \"type\": \"boolean\"\n            },\n            \"deleteObjectsFromSourceAfterTransfer\": {\n              \"type\": \"boolean\"\n            },\n            \"deleteObjectsUniqueInSink\": {\n              \"type\": \"boolean\"\n            }\n          }\n        }\n      }\n    },\n    \"GcsData\": {\n      \"type\": \"object\",\n      \"description\": \"Google Cloud Storage bucket reference\",\n      \"required\": [\"bucketName\"],\n      \"properties\": {\n        \"bucketName\": {\n          \"type\": \"string\",\n          \"description\": \"Cloud Storage bucket name\"\n        },\n        \"path\": {\n          \"type\": \"string\",\n          \"description\": \"Root path to transfer objects\"\n        }\n      }\n\
  \    },\n    \"AwsS3Data\": {\n      \"type\": \"object\",\n      \"description\": \"Amazon S3 bucket reference\",\n      \"required\": [\"bucketName\"],\n      \"properties\": {\n        \"bucketName\": {\n          \"type\": \"string\",\n          \"description\": \"S3 bucket name\"\n        },\n        \"path\": {\n          \"type\": \"string\",\n          \"description\": \"Root path within the bucket\"\n        },\n        \"roleArn\": {\n          \"type\": \"string\",\n          \"description\": \"AWS IAM role ARN for cross-account access\"\n        }\n      }\n    },\n    \"AzureBlobStorageData\": {\n      \"type\": \"object\",\n      \"description\": \"Azure Blob Storage container reference\",\n      \"required\": [\"storageAccount\", \"container\"],\n      \"properties\": {\n        \"storageAccount\": {\n          \"type\": \"string\",\n          \"description\": \"Azure storage account name\"\n        },\n        \"container\": {\n          \"type\": \"string\",\n        \
  \  \"description\": \"Azure Blob Storage container name\"\n        },\n        \"path\": {\n          \"type\": \"string\",\n          \"description\": \"Root path within the container\"\n        }\n      }\n    },\n    \"Schedule\": {\n      \"type\": \"object\",\n      \"description\": \"Transfer schedule configuration\",\n      \"properties\": {\n        \"scheduleStartDate\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"year\": { \"type\": \"integer\" },\n            \"month\": { \"type\": \"integer\" },\n            \"day\": { \"type\": \"integer\" }\n          }\n        },\n        \"scheduleEndDate\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"year\": { \"type\": \"integer\" },\n            \"month\": { \"type\": \"integer\" },\n            \"day\": { \"type\": \"integer\" }\n          }\n        },\n        \"repeatInterval\": {\n          \"type\": \"string\",\n          \"description\": \"Interval between\
  \ runs in seconds format (e.g., 86400s)\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-transfer-service/refs/heads/main/json-schema/google-cloud-transfer-service-job-schema.json
tags:
- Azure
- Cloud Storage
- Data Transfer
- Migration
- S3
- Storage
title: Google Cloud Storage Transfer Job
---
