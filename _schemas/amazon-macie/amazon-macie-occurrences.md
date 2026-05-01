---
description: Specifies the location of 1-15 occurrences of sensitive data that was detected by a managed data identifier or a custom data identifier and produced a sensitive data finding.
layout: schema
name: Occurrences
properties_list:
- description: ''
  name: cells
  type: object
- description: ''
  name: lineRanges
  type: object
- description: ''
  name: offsetRanges
  type: object
- description: ''
  name: pages
  type: object
- description: ''
  name: records
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-occurrences-schema.json
slug: amazon-macie-occurrences
source_filename: amazon-macie-occurrences-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-occurrences-schema.json\",\n  \"title\": \"Occurrences\",\n  \"description\": \"Specifies the location of 1-15 occurrences of sensitive data that was detected by a managed data identifier or a custom data identifier and produced a sensitive data finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cells\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Cells\"\n        },\n        {\n          \"description\": \"<p>An array of objects, one for each occurrence of sensitive data in a Microsoft Excel workbook, CSV file, or TSV file. This value is null for all other types of files.</p> <p>Each Cell object specifies a cell or field that contains the sensitive data.</p>\"\n        }\n      ]\n    },\n    \"lineRanges\": {\n      \"allOf\": [\n        {\n  \
  \        \"$ref\": \"#/components/schemas/Ranges\"\n        },\n        {\n          \"description\": \"<p>An array of objects, one for each occurrence of sensitive data in an email message or a non-binary text file such as an HTML, TXT, or XML file. Each Range object specifies a line or inclusive range of lines that contains the sensitive data, and the position of the data on the specified line or lines.</p> <p>This value is often null for file types that are supported by Cell, Page, or Record objects. Exceptions are the location of sensitive data in: unstructured sections of an otherwise structured file, such as a comment in a file; a malformed file that Amazon Macie analyzes as plain text; and, a CSV or TSV file that has any column names that contain sensitive data.</p>\"\n        }\n      ]\n    },\n    \"offsetRanges\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ranges\"\n        },\n        {\n          \"description\": \" <p>Reserved for future\
  \ use.</p>\"\n        }\n      ]\n    },\n    \"pages\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Pages\"\n        },\n        {\n          \"description\": \"<p>An array of objects, one for each occurrence of sensitive data in an Adobe Portable Document Format file. This value is null for all other types of files.</p> <p>Each Page object specifies a page that contains the sensitive data.</p>\"\n        }\n      ]\n    },\n    \"records\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Records\"\n        },\n        {\n          \"description\": \"<p>An array of objects, one for each occurrence of sensitive data in an Apache Avro object container, Apache Parquet file, JSON file, or JSON Lines file. This value is null for all other types of files.</p> <p>For an Avro object container or Parquet file, each Record object specifies a record index and the path to a field in a record that contains the sensitive data. For a JSON\
  \ or JSON Lines file, each Record object specifies the path to a field or array that contains the sensitive data. For a JSON Lines file, it also specifies the index of the line that contains the data.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-occurrences-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: Occurrences
---
