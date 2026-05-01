---
description: ExportJournalToS3Response schema from Amazon QLDB API
layout: schema
name: ExportJournalToS3Response
properties_list:
- description: ''
  name: ExportId
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-export-journal-to-s3response-schema.json
slug: amazon-qldb-export-journal-to-s3response
source_filename: amazon-qldb-export-journal-to-s3response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-export-journal-to-s3response-schema.json\",\n  \"title\": \"ExportJournalToS3Response\",\n  \"description\": \"ExportJournalToS3Response schema from Amazon QLDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ExportId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UniqueId\"\n        },\n        {\n          \"description\": \"<p>The UUID (represented in Base62-encoded text) that QLDB assigns to each journal export job.</p> <p>To describe your export request and check the status of the job, you can use <code>ExportId</code> to call <code>DescribeJournalS3Export</code>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ExportId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-export-journal-to-s3response-schema.json
tags:
- Blockchain
- Database
- Ledger
title: ExportJournalToS3Response
---
