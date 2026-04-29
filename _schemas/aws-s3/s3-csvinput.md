---
description: Describes how an uncompressed comma-separated values (CSV)-formatted input object is formatted.
layout: schema
name: CSVInput
properties_list:
- description: ''
  name: FileHeaderInfo
  type: object
- description: ''
  name: Comments
  type: object
- description: ''
  name: QuoteEscapeCharacter
  type: object
- description: ''
  name: RecordDelimiter
  type: object
- description: ''
  name: FieldDelimiter
  type: object
- description: ''
  name: QuoteCharacter
  type: object
- description: ''
  name: AllowQuotedRecordDelimiter
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-csvinput-schema.json
slug: s3-csvinput
source_filename: s3-csvinput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CSVInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileHeaderInfo\": {},\n    \"Comments\": {},\n    \"QuoteEscapeCharacter\": {},\n    \"RecordDelimiter\": {},\n    \"FieldDelimiter\": {},\n    \"QuoteCharacter\": {},\n    \"AllowQuotedRecordDelimiter\": {}\n  },\n  \"description\": \"Describes how an uncompressed comma-separated values (CSV)-formatted input object is formatted.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-csvinput-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: CSVInput
---
