---
description: SqlRecords schema from Amazon Redshift
layout: schema
name: SqlRecords
properties_list: []
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-data-sql-records-schema.json
slug: redshift-data-sql-records
source_filename: redshift-data-sql-records-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"array\",\n    \"items\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"blobValue\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Blob\"\n            },\n            {\n              \"description\": \"A value of the BLOB data type. \"\n            }\n          ]\n        },\n        \"booleanValue\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/BoxedBoolean\"\n            },\n            {\n              \"description\": \"A value of the Boolean data type. \"\n            }\n          ]\n        },\n        \"doubleValue\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/BoxedDouble\"\n            },\n            {\n              \"description\": \"A value of the double data type. \"\n            }\n          ]\n        },\n        \"isNull\": {\n          \"allOf\": [\n\
  \            {\n              \"$ref\": \"#/components/schemas/BoxedBoolean\"\n            },\n            {\n              \"description\": \"A value that indicates whether the data is NULL. \"\n            }\n          ]\n        },\n        \"longValue\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/BoxedLong\"\n            },\n            {\n              \"description\": \"A value of the long data type. \"\n            }\n          ]\n        },\n        \"stringValue\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/String\"\n            },\n            {\n              \"description\": \"A value of the string data type. \"\n            }\n          ]\n        }\n      },\n      \"description\": \"A data value in a column. \"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-sql-records-schema.json\"\
  ,\n  \"title\": \"SqlRecords\",\n  \"description\": \"SqlRecords schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-sql-records-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: SqlRecords
---
