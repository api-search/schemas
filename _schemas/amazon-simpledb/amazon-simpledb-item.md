---
description: ''
layout: schema
name: Item
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: AlternateNameEncoding
  type: object
- description: ''
  name: Attributes
  type: object
provider_name: Amazon SimpleDB
provider_slug: amazon-simpledb
schema_file: json-schema/amazon-simpledb-item-schema.json
slug: amazon-simpledb-item
source_filename: amazon-simpledb-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-item-schema.json\",\n  \"title\": \"Item\",\n  \"description\": \"\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the item.\"\n        }\n      ]\n    },\n    \"AlternateNameEncoding\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"\"\n        }\n      ]\n    },\n    \"Attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeList\"\n        },\n        {\n          \"description\": \"A list of attributes.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Attributes\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-item-schema.json
tags:
- Cloud Storage
- Data Storage
- Database
- NoSQL
title: Item
---
