---
description: ''
layout: schema
name: Attribute
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: AlternateNameEncoding
  type: object
- description: ''
  name: Value
  type: object
- description: ''
  name: AlternateValueEncoding
  type: object
provider_name: Amazon SimpleDB
provider_slug: amazon-simpledb
schema_file: json-schema/amazon-simpledb-attribute-schema.json
slug: amazon-simpledb-attribute
source_filename: amazon-simpledb-attribute-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-attribute-schema.json\",\n  \"title\": \"Attribute\",\n  \"description\": \"\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the attribute.\"\n        }\n      ]\n    },\n    \"AlternateNameEncoding\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The value of the attribute.\"\n        }\n      ]\n    },\n    \"AlternateValueEncoding\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-attribute-schema.json
tags:
- AWS
- Cloud Storage
- Data Storage
- Database
- NoSQL
title: Attribute
---
