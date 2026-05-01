---
description: The Amazon Simple Storage Service (Amazon S3) bucket location in which a journal export job writes the journal contents.
layout: schema
name: S3ExportConfiguration
properties_list:
- description: ''
  name: Bucket
  type: object
- description: ''
  name: Prefix
  type: object
- description: ''
  name: EncryptionConfiguration
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-s3export-configuration-schema.json
slug: amazon-qldb-s3export-configuration
source_filename: amazon-qldb-s3export-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-s3export-configuration-schema.json\",\n  \"title\": \"S3ExportConfiguration\",\n  \"description\": \"The Amazon Simple Storage Service (Amazon S3) bucket location in which a journal export job writes the journal contents.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Bucket\"\n        },\n        {\n          \"description\": \"<p>The Amazon S3 bucket name in which a journal export job writes the journal contents.</p> <p>The bucket name must comply with the Amazon S3 bucket naming conventions. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/BucketRestrictions.html\\\">Bucket Restrictions and Limitations</a> in the <i>Amazon S3 Developer Guide</i>.</p>\"\n    \
  \    }\n      ]\n    },\n    \"Prefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Prefix\"\n        },\n        {\n          \"description\": \"<p>The prefix for the Amazon S3 bucket in which a journal export job writes the journal contents.</p> <p>The prefix must comply with Amazon S3 key naming rules and restrictions. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingMetadata.html\\\">Object Key and Metadata</a> in the <i>Amazon S3 Developer Guide</i>.</p> <p>The following are examples of valid <code>Prefix</code> values:</p> <ul> <li> <p> <code>JournalExports-ForMyLedger/Testing/</code> </p> </li> <li> <p> <code>JournalExports</code> </p> </li> <li> <p> <code>My:Tests/</code> </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"EncryptionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3EncryptionConfiguration\"\n        },\n        {\n          \"description\"\
  : \"The encryption settings that are used by a journal export job to write data in an Amazon S3 bucket.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Bucket\",\n    \"Prefix\",\n    \"EncryptionConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-s3export-configuration-schema.json
tags:
- Blockchain
- Database
- Ledger
title: S3ExportConfiguration
---
