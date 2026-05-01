---
description: Information about a journal export job, including the ledger name, export ID, creation time, current status, and the parameters of the original export creation request.
layout: schema
name: JournalS3ExportDescription
properties_list:
- description: ''
  name: LedgerName
  type: object
- description: ''
  name: ExportId
  type: object
- description: ''
  name: ExportCreationTime
  type: object
- description: ''
  name: Status
  type: object
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
schema_file: json-schema/amazon-qldb-journal-s3export-description-schema.json
slug: amazon-qldb-journal-s3export-description
source_filename: amazon-qldb-journal-s3export-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-journal-s3export-description-schema.json\",\n  \"title\": \"JournalS3ExportDescription\",\n  \"description\": \"Information about a journal export job, including the ledger name, export ID, creation time, current status, and the parameters of the original export creation request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LedgerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LedgerName\"\n        },\n        {\n          \"description\": \"The name of the ledger.\"\n        }\n      ]\n    },\n    \"ExportId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UniqueId\"\n        },\n        {\n          \"description\": \"The UUID (represented in Base62-encoded text) of the journal export job.\"\n        }\n      ]\n\
  \    },\n    \"ExportCreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time, in epoch time format, when the export job was created. (Epoch time format is the number of seconds elapsed since 12:00:00 AM January 1, 1970 UTC.)\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExportStatus\"\n        },\n        {\n          \"description\": \"The current state of the journal export job.\"\n        }\n      ]\n    },\n    \"InclusiveStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The inclusive start date and time for the range of journal contents that was specified in the original export request.\"\n        }\n      ]\n    },\n    \"ExclusiveEndTime\": {\n      \"allOf\": [\n        {\n      \
  \    \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The exclusive end date and time for the range of journal contents that was specified in the original export request.\"\n        }\n      ]\n    },\n    \"S3ExportConfiguration\": {\n      \"$ref\": \"#/components/schemas/S3ExportConfiguration\"\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the IAM role that grants QLDB permissions for a journal export job to do the following:</p> <ul> <li> <p>Write objects into your Amazon Simple Storage Service (Amazon S3) bucket.</p> </li> <li> <p>(Optional) Use your customer managed key in Key Management Service (KMS) for server-side encryption of your exported data.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"OutputFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputFormat\"\
  \n        },\n        {\n          \"description\": \"The output format of the exported journal data.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LedgerName\",\n    \"ExportId\",\n    \"ExportCreationTime\",\n    \"Status\",\n    \"InclusiveStartTime\",\n    \"ExclusiveEndTime\",\n    \"S3ExportConfiguration\",\n    \"RoleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-journal-s3export-description-schema.json
tags:
- Blockchain
- Database
- Ledger
title: JournalS3ExportDescription
---
