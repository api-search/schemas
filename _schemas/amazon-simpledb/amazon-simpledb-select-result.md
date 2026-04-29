---
description: SelectResult schema from Amazon SimpleDB API
layout: schema
name: SelectResult
properties_list:
- description: ''
  name: Items
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon SimpleDB
provider_slug: amazon-simpledb
schema_file: json-schema/amazon-simpledb-select-result-schema.json
slug: amazon-simpledb-select-result
source_filename: amazon-simpledb-select-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-select-result-schema.json\",\n  \"title\": \"SelectResult\",\n  \"description\": \"SelectResult schema from Amazon SimpleDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Items\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ItemList\"\n        },\n        {\n          \"description\": \"A list of items that match the select expression.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"An opaque token indicating that more items than <code>MaxNumberOfItems</code> were matched, the response size exceeded 1 megabyte, or the execution time exceeded 5 seconds.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-select-result-schema.json
tags:
- AWS
- Cloud Storage
- Data Storage
- Database
- NoSQL
title: SelectResult
---
