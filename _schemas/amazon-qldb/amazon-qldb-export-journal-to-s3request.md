---
description: ExportJournalToS3Request schema from Amazon QLDB API
layout: schema
name: ExportJournalToS3Request
properties_list:
- description: ''
  name: InclusiveStartTime
  type: object
- description: ''
  name: ExclusiveEndTime
  type: object
- description: ''
  name: S3ExportConfiguration
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: OutputFormat
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-export-journal-to-s3request-schema.json
slug: amazon-qldb-export-journal-to-s3request
source_filename: amazon-qldb-export-journal-to-s3request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-export-journal-to-s3request-schema.json\",\n  \"title\": \"ExportJournalToS3Request\",\n  \"description\": \"ExportJournalToS3Request schema from Amazon QLDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InclusiveStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"<p>The inclusive start date and time for the range of journal contents to export.</p> <p>The <code>InclusiveStartTime</code> must be in <code>ISO 8601</code> date and time format and in Universal Coordinated Time (UTC). For example: <code>2019-06-13T21:36:34Z</code>.</p> <p>The <code>InclusiveStartTime</code> must be before <code>ExclusiveEndTime</code>.</p> <p>If you provide an <code>InclusiveStartTime</code> that is before\
  \ the ledger's <code>CreationDateTime</code>, Amazon QLDB defaults it to the ledger's <code>CreationDateTime</code>.</p>\"\n        }\n      ]\n    },\n    \"ExclusiveEndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"<p>The exclusive end date and time for the range of journal contents to export.</p> <p>The <code>ExclusiveEndTime</code> must be in <code>ISO 8601</code> date and time format and in Universal Coordinated Time (UTC). For example: <code>2019-06-13T21:36:34Z</code>.</p> <p>The <code>ExclusiveEndTime</code> must be less than or equal to the current UTC date and time.</p>\"\n        }\n      ]\n    },\n    \"S3ExportConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ExportConfiguration\"\n        },\n        {\n          \"description\": \"The configuration settings of the Amazon S3 bucket destination for your export request.\"\n  \
  \      }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the IAM role that grants QLDB permissions for a journal export job to do the following:</p> <ul> <li> <p>Write objects into your Amazon Simple Storage Service (Amazon S3) bucket.</p> </li> <li> <p>(Optional) Use your customer managed key in Key Management Service (KMS) for server-side encryption of your exported data.</p> </li> </ul> <p>To pass a role to QLDB when requesting a journal export, you must have permissions to perform the <code>iam:PassRole</code> action on the IAM role resource. This is required for all journal export requests.</p>\"\n        }\n      ]\n    },\n    \"OutputFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputFormat\"\n        },\n        {\n          \"description\": \"The output format of your exported\
  \ journal data. If this parameter is not specified, the exported data defaults to <code>ION_TEXT</code> format.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InclusiveStartTime\",\n    \"ExclusiveEndTime\",\n    \"S3ExportConfiguration\",\n    \"RoleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-export-journal-to-s3request-schema.json
tags:
- Blockchain
- Database
- Ledger
title: ExportJournalToS3Request
---
