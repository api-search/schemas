---
description: StartMailboxExportJobRequest schema from Amazon WorkMail API
layout: schema
name: StartMailboxExportJobRequest
properties_list:
- description: ''
  name: ClientToken
  type: object
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: EntityId
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: KmsKeyArn
  type: object
- description: ''
  name: S3BucketName
  type: object
- description: ''
  name: S3Prefix
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-start-mailbox-export-job-request-schema.json
slug: workmail-start-mailbox-export-job-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ClientToken\",\n    \"OrganizationId\",\n    \"EntityId\",\n    \"RoleArn\",\n    \"KmsKeyArn\",\n    \"S3BucketName\",\n    \"S3Prefix\"\n  ],\n  \"title\": \"StartMailboxExportJobRequest\",\n  \"properties\": {\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdempotencyClientToken\"\n        },\n        {\n          \"description\": \"The idempotency token for the client request.\"\n        }\n      ]\n    },\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The identifier associated with the organization.\"\n        }\n      ]\n    },\n    \"EntityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The identifier of the user or resource associated\
  \ with the mailbox.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The mailbox export job description.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The ARN of the AWS Identity and Access Management (IAM) role that grants write permission to the S3 bucket.\"\n        }\n      ]\n    },\n    \"KmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the symmetric AWS Key Management Service (AWS KMS) key that encrypts the exported mailbox content.\"\n        }\n      ]\n    },\n    \"S3BucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3BucketName\"\
  \n        },\n        {\n          \"description\": \"The name of the S3 bucket.\"\n        }\n      ]\n    },\n    \"S3Prefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ObjectKey\"\n        },\n        {\n          \"description\": \"The S3 bucket prefix.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-start-mailbox-export-job-request-schema.json\",\n  \"description\": \"StartMailboxExportJobRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-start-mailbox-export-job-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: StartMailboxExportJobRequest
---
