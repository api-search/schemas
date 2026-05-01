---
description: Specifies a property-based condition that determines whether an S3 object is included or excluded from a classification job.
layout: schema
name: SimpleScopeTerm
properties_list:
- description: ''
  name: comparator
  type: object
- description: ''
  name: key
  type: object
- description: ''
  name: values
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-simple-scope-term-schema.json
slug: amazon-macie-simple-scope-term
source_filename: amazon-macie-simple-scope-term-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-simple-scope-term-schema.json\",\n  \"title\": \"SimpleScopeTerm\",\n  \"description\": \"Specifies a property-based condition that determines whether an S3 object is included or excluded from a classification job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"comparator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobComparator\"\n        },\n        {\n          \"description\": \"<p>The operator to use in the condition. Valid values for each supported property (key) are:</p> <ul><li><p>OBJECT_EXTENSION - EQ (equals) or NE (not equals)</p></li> <li><p>OBJECT_KEY - STARTS_WITH</p></li> <li><p>OBJECT_LAST_MODIFIED_DATE - Any operator except CONTAINS</p></li> <li><p>OBJECT_SIZE - Any operator except CONTAINS</p></li></ul>\"\n        }\n      ]\n   \
  \ },\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScopeFilterKey\"\n        },\n        {\n          \"description\": \"The object property to use in the condition.\"\n        }\n      ]\n    },\n    \"values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"<p>An array that lists the values to use in the condition. If the value for the key property is OBJECT_EXTENSION or OBJECT_KEY, this array can specify multiple values and Amazon Macie uses OR logic to join the values. Otherwise, this array can specify only one value.</p> <p>Valid values for each supported property (key) are:</p> <ul><li><p>OBJECT_EXTENSION - A string that represents the file name extension of an object. For example: docx or pdf</p></li> <li><p>OBJECT_KEY - A string that represents the key prefix (folder name or path) of an object. For example: logs or awslogs/eventlogs.\
  \ This value applies a condition to objects whose keys (names) begin with the specified value.</p></li> <li><p>OBJECT_LAST_MODIFIED_DATE - The date and time (in UTC and extended ISO 8601 format) when an object was created or last changed, whichever is latest. For example: 2020-09-28T14:31:13Z</p></li> <li><p>OBJECT_SIZE - An integer that represents the storage size (in bytes) of an object.</p></li></ul> <p>Macie doesn't support use of wildcard characters in these values. Also, string values are case sensitive.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-simple-scope-term-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: SimpleScopeTerm
---
