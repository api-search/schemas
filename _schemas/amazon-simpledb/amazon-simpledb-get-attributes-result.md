---
description: GetAttributesResult schema from Amazon SimpleDB API
layout: schema
name: GetAttributesResult
properties_list:
- description: ''
  name: Attributes
  type: object
provider_name: Amazon SimpleDB
provider_slug: amazon-simpledb
schema_file: json-schema/amazon-simpledb-get-attributes-result-schema.json
slug: amazon-simpledb-get-attributes-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-get-attributes-result-schema.json\",\n  \"title\": \"GetAttributesResult\",\n  \"description\": \"GetAttributesResult schema from Amazon SimpleDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeList\"\n        },\n        {\n          \"description\": \"The list of attributes returned by the operation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-get-attributes-result-schema.json
tags:
- AWS
- Cloud Storage
- Data Storage
- Database
- NoSQL
title: GetAttributesResult
---
