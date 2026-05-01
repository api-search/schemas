---
description: DescribeJournalS3ExportResponse schema from Amazon QLDB API
layout: schema
name: DescribeJournalS3ExportResponse
properties_list:
- description: ''
  name: ExportDescription
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-describe-journal-s3export-response-schema.json
slug: amazon-qldb-describe-journal-s3export-response
source_filename: amazon-qldb-describe-journal-s3export-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-describe-journal-s3export-response-schema.json\",\n  \"title\": \"DescribeJournalS3ExportResponse\",\n  \"description\": \"DescribeJournalS3ExportResponse schema from Amazon QLDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ExportDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JournalS3ExportDescription\"\n        },\n        {\n          \"description\": \"Information about the journal export job returned by a <code>DescribeJournalS3Export</code> request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ExportDescription\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-describe-journal-s3export-response-schema.json
tags:
- Blockchain
- Database
- Ledger
title: DescribeJournalS3ExportResponse
---
