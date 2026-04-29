---
description: ConfigurationsMap schema from AWS IAM Access Analyzer API
layout: schema
name: ConfigurationsMap
properties_list: []
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-configurations-map-schema.json
slug: iam-access-analyzer-configurations-map
source_filename: iam-access-analyzer-configurations-map-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-configurations-map-schema.json\",\n  \"title\": \"ConfigurationsMap\",\n  \"description\": \"ConfigurationsMap schema from AWS IAM Access Analyzer API\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"ebsSnapshot\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/EbsSnapshotConfiguration\"\n          },\n          {\n            \"description\": \"The access control configuration is for an Amazon EBS volume snapshot.\"\n          }\n        ]\n      },\n      \"ecrRepository\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/EcrRepositoryConfiguration\"\n          },\n          {\n            \"description\": \"The access control configuration\
  \ is for an Amazon ECR repository.\"\n          }\n        ]\n      },\n      \"iamRole\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/IamRoleConfiguration\"\n          },\n          {\n            \"description\": \"The access control configuration is for an IAM role. \"\n          }\n        ]\n      },\n      \"efsFileSystem\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/EfsFileSystemConfiguration\"\n          },\n          {\n            \"description\": \"The access control configuration is for an Amazon EFS file system.\"\n          }\n        ]\n      },\n      \"kmsKey\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/KmsKeyConfiguration\"\n          },\n          {\n            \"description\": \"The access control configuration is for a KMS key. \"\n          }\n        ]\n      },\n      \"rdsDbClusterSnapshot\": {\n        \"allOf\": [\n          {\n           \
  \ \"$ref\": \"#/components/schemas/RdsDbClusterSnapshotConfiguration\"\n          },\n          {\n            \"description\": \"The access control configuration is for an Amazon RDS DB cluster snapshot.\"\n          }\n        ]\n      },\n      \"rdsDbSnapshot\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/RdsDbSnapshotConfiguration\"\n          },\n          {\n            \"description\": \"The access control configuration is for an Amazon RDS DB snapshot.\"\n          }\n        ]\n      },\n      \"secretsManagerSecret\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/SecretsManagerSecretConfiguration\"\n          },\n          {\n            \"description\": \"The access control configuration is for a Secrets Manager secret.\"\n          }\n        ]\n      },\n      \"s3Bucket\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/S3BucketConfiguration\"\n          },\n  \
  \        {\n            \"description\": \"The access control configuration is for an Amazon S3 Bucket. \"\n          }\n        ]\n      },\n      \"snsTopic\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/SnsTopicConfiguration\"\n          },\n          {\n            \"description\": \"The access control configuration is for an Amazon SNS topic\"\n          }\n        ]\n      },\n      \"sqsQueue\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/SqsQueueConfiguration\"\n          },\n          {\n            \"description\": \"The access control configuration is for an Amazon SQS queue. \"\n          }\n        ]\n      }\n    },\n    \"description\": \"Access control configuration structures for your resource. You specify the configuration as a type-value pair. You can specify only one type of access control configuration.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-configurations-map-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: ConfigurationsMap
---
