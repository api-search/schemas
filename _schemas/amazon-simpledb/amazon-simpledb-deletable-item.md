---
description: DeletableItem schema from Amazon SimpleDB API
layout: schema
name: DeletableItem
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Attributes
  type: object
provider_name: Amazon SimpleDB
provider_slug: amazon-simpledb
schema_file: json-schema/amazon-simpledb-deletable-item-schema.json
slug: amazon-simpledb-deletable-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-deletable-item-schema.json\",\n  \"title\": \"DeletableItem\",\n  \"description\": \"DeletableItem schema from Amazon SimpleDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ItemName\"\n          }\n        }\n      ]\n    },\n    \"Attributes\": {\n      \"$ref\": \"#/components/schemas/DeletableAttributeList\"\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-deletable-item-schema.json
tags:
- AWS
- Cloud Storage
- Data Storage
- Database
- NoSQL
title: DeletableItem
---
