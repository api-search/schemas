---
description: BatchPutAttributesRequest schema from Amazon SimpleDB API
layout: schema
name: BatchPutAttributesRequest
properties_list:
- description: ''
  name: DomainName
  type: object
- description: ''
  name: Items
  type: object
provider_name: Amazon SimpleDB
provider_slug: amazon-simpledb
schema_file: json-schema/amazon-simpledb-batch-put-attributes-request-schema.json
slug: amazon-simpledb-batch-put-attributes-request
source_filename: amazon-simpledb-batch-put-attributes-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-batch-put-attributes-request-schema.json\",\n  \"title\": \"BatchPutAttributesRequest\",\n  \"description\": \"BatchPutAttributesRequest schema from Amazon SimpleDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the domain in which the attributes are being stored.\"\n        }\n      ]\n    },\n    \"Items\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReplaceableItemList\"\n        },\n        {\n          \"description\": \"A list of items on which to perform the operation.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DomainName\",\n    \"Items\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-batch-put-attributes-request-schema.json
tags:
- AWS
- Cloud Storage
- Data Storage
- Database
- NoSQL
title: BatchPutAttributesRequest
---
