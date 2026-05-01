---
description: DescribeMailboxExportJobResponse schema from Amazon WorkMail API
layout: schema
name: DescribeMailboxExportJobResponse
properties_list:
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
- description: ''
  name: S3Path
  type: object
- description: ''
  name: EstimatedProgress
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: ErrorInfo
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: EndTime
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-describe-mailbox-export-job-response-schema.json
slug: workmail-describe-mailbox-export-job-response
source_filename: workmail-describe-mailbox-export-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"EntityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The identifier of the user or resource associated with the mailbox.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The mailbox export job description.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The ARN of the AWS Identity and Access Management (IAM) role that grants write permission to the Amazon Simple Storage Service (Amazon S3) bucket.\"\n        }\n      ]\n    },\n    \"KmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyArn\"\
  \n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the symmetric AWS Key Management Service (AWS KMS) key that encrypts the exported mailbox content.\"\n        }\n      ]\n    },\n    \"S3BucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3BucketName\"\n        },\n        {\n          \"description\": \"The name of the S3 bucket.\"\n        }\n      ]\n    },\n    \"S3Prefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ObjectKey\"\n        },\n        {\n          \"description\": \"The S3 bucket prefix.\"\n        }\n      ]\n    },\n    \"S3Path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ObjectKey\"\n        },\n        {\n          \"description\": \"The path to the S3 bucket and file that the mailbox export job is exporting to.\"\n        }\n      ]\n    },\n    \"EstimatedProgress\": {\n      \"allOf\": [\n        {\n         \
  \ \"$ref\": \"#/components/schemas/Percentage\"\n        },\n        {\n          \"description\": \"The estimated progress of the mailbox export job, in percentage points.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MailboxExportJobState\"\n        },\n        {\n          \"description\": \"The state of the mailbox export job.\"\n        }\n      ]\n    },\n    \"ErrorInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MailboxExportErrorInfo\"\n        },\n        {\n          \"description\": \"Error information for failed mailbox export jobs.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The mailbox export job start timestamp.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The mailbox export job end timestamp.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeMailboxExportJobResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-describe-mailbox-export-job-response-schema.json\",\n  \"description\": \"DescribeMailboxExportJobResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-describe-mailbox-export-job-response-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DescribeMailboxExportJobResponse
---
