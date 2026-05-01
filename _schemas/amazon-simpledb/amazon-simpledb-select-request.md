---
description: SelectRequest schema from Amazon SimpleDB API
layout: schema
name: SelectRequest
properties_list:
- description: ''
  name: SelectExpression
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: ConsistentRead
  type: object
provider_name: Amazon SimpleDB
provider_slug: amazon-simpledb
schema_file: json-schema/amazon-simpledb-select-request-schema.json
slug: amazon-simpledb-select-request
source_filename: amazon-simpledb-select-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-select-request-schema.json\",\n  \"title\": \"SelectRequest\",\n  \"description\": \"SelectRequest schema from Amazon SimpleDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SelectExpression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The expression used to query the domain.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A string informing Amazon SimpleDB where to start the next list of <code>ItemNames</code>.\"\n        }\n      ]\n    },\n    \"ConsistentRead\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\
  \n        },\n        {\n          \"description\": \"Determines whether or not strong consistency should be enforced when data is read from SimpleDB. If <code>true</code>, any data previously written to SimpleDB will be returned. Otherwise, results will be consistent eventually, and the client may not see data that was written immediately before your read.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SelectExpression\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-select-request-schema.json
tags:
- Cloud Storage
- Data Storage
- Database
- NoSQL
title: SelectRequest
---
