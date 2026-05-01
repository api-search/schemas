---
description: GetAttributesRequest schema from Amazon SimpleDB API
layout: schema
name: GetAttributesRequest
properties_list:
- description: ''
  name: DomainName
  type: object
- description: ''
  name: ItemName
  type: object
- description: ''
  name: AttributeNames
  type: object
- description: ''
  name: ConsistentRead
  type: object
provider_name: Amazon SimpleDB
provider_slug: amazon-simpledb
schema_file: json-schema/amazon-simpledb-get-attributes-request-schema.json
slug: amazon-simpledb-get-attributes-request
source_filename: amazon-simpledb-get-attributes-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-get-attributes-request-schema.json\",\n  \"title\": \"GetAttributesRequest\",\n  \"description\": \"GetAttributesRequest schema from Amazon SimpleDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the domain in which to perform the operation.\"\n        }\n      ]\n    },\n    \"ItemName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the item.\"\n        }\n      ]\n    },\n    \"AttributeNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeNameList\"\n        },\n \
  \       {\n          \"description\": \"The names of the attributes.\"\n        }\n      ]\n    },\n    \"ConsistentRead\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Determines whether or not strong consistency should be enforced when data is read from SimpleDB. If <code>true</code>, any data previously written to SimpleDB will be returned. Otherwise, results will be consistent eventually, and the client may not see data that was written immediately before your read.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DomainName\",\n    \"ItemName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-get-attributes-request-schema.json
tags:
- Cloud Storage
- Data Storage
- Database
- NoSQL
title: GetAttributesRequest
---
