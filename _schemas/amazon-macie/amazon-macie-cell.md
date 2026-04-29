---
description: Specifies the location of an occurrence of sensitive data in a Microsoft Excel workbook, CSV file, or TSV file.
layout: schema
name: Cell
properties_list:
- description: ''
  name: cellReference
  type: object
- description: ''
  name: column
  type: object
- description: ''
  name: columnName
  type: object
- description: ''
  name: row
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-cell-schema.json
slug: amazon-macie-cell
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-cell-schema.json\",\n  \"title\": \"Cell\",\n  \"description\": \"Specifies the location of an occurrence of sensitive data in a Microsoft Excel workbook, CSV file, or TSV file.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cellReference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The location of the cell, as an absolute cell reference, that contains the sensitive data, for example Sheet2!C5 for cell C5 on Sheet2 in a Microsoft Excel workbook. This value is null for CSV and TSV files.\"\n        }\n      ]\n    },\n    \"column\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The column number\
  \ of the column that contains the sensitive data. For a Microsoft Excel workbook, this value correlates to the alphabetical character(s) for a column identifier, for example: 1 for column A, 2 for column B, and so on.\"\n        }\n      ]\n    },\n    \"columnName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the column that contains the sensitive data, if available.\"\n        }\n      ]\n    },\n    \"row\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The row number of the row that contains the sensitive data.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-cell-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: Cell
---
