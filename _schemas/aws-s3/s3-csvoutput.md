---
description: Describes how uncompressed comma-separated values (CSV)-formatted results are formatted.
layout: schema
name: CSVOutput
properties_list:
- description: ''
  name: QuoteFields
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
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-csvoutput-schema.json
slug: s3-csvoutput
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CSVOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"QuoteFields\": {},\n    \"QuoteEscapeCharacter\": {},\n    \"RecordDelimiter\": {},\n    \"FieldDelimiter\": {},\n    \"QuoteCharacter\": {}\n  },\n  \"description\": \"Describes how uncompressed comma-separated values (CSV)-formatted results are formatted.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-csvoutput-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: CSVOutput
---
