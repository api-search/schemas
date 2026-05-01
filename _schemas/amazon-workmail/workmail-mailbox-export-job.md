---
description: The details of a mailbox export job, including the user or resource ID associated with the mailbox and the S3 bucket that the mailbox contents are exported to.
layout: schema
name: MailboxExportJob
properties_list:
- description: ''
  name: JobId
  type: object
- description: ''
  name: EntityId
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: S3BucketName
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
  name: StartTime
  type: object
- description: ''
  name: EndTime
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-mailbox-export-job-schema.json
slug: workmail-mailbox-export-job
source_filename: workmail-mailbox-export-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MailboxExportJobId\"\n        },\n        {\n          \"description\": \"The identifier of the mailbox export job.\"\n        }\n      ]\n    },\n    \"EntityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The identifier of the user or resource associated with the mailbox.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The mailbox export job description.\"\n        }\n      ]\n    },\n    \"S3BucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3BucketName\"\n        },\n        {\n          \"description\": \"The name of the S3 bucket.\"\n  \
  \      }\n      ]\n    },\n    \"S3Path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ObjectKey\"\n        },\n        {\n          \"description\": \"The path to the S3 bucket and file that the mailbox export job exports to.\"\n        }\n      ]\n    },\n    \"EstimatedProgress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Percentage\"\n        },\n        {\n          \"description\": \"The estimated progress of the mailbox export job, in percentage points.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MailboxExportJobState\"\n        },\n        {\n          \"description\": \"The state of the mailbox export job.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The mailbox export job start timestamp.\"\
  \n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The mailbox export job end timestamp.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The details of a mailbox export job, including the user or resource ID associated with the mailbox and the S3 bucket that the mailbox contents are exported to.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MailboxExportJob\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-mailbox-export-job-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-mailbox-export-job-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: MailboxExportJob
---
