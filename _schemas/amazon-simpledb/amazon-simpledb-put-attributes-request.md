---
description: PutAttributesRequest schema from Amazon SimpleDB API
layout: schema
name: PutAttributesRequest
properties_list:
- description: ''
  name: DomainName
  type: object
- description: ''
  name: ItemName
  type: object
- description: ''
  name: Attributes
  type: object
- description: ''
  name: Expected
  type: object
provider_name: Amazon SimpleDB
provider_slug: amazon-simpledb
schema_file: json-schema/amazon-simpledb-put-attributes-request-schema.json
slug: amazon-simpledb-put-attributes-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-put-attributes-request-schema.json\",\n  \"title\": \"PutAttributesRequest\",\n  \"description\": \"PutAttributesRequest schema from Amazon SimpleDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the domain in which to perform the operation.\"\n        }\n      ]\n    },\n    \"ItemName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the item.\"\n        }\n      ]\n    },\n    \"Attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReplaceableAttributeList\"\n        },\n\
  \        {\n          \"description\": \"The list of attributes.\"\n        }\n      ]\n    },\n    \"Expected\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateCondition\"\n        },\n        {\n          \"description\": \"The update condition which, if specified, determines whether the specified attributes will be updated or not. The update condition must be satisfied in order for this request to be processed and the attributes to be updated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DomainName\",\n    \"ItemName\",\n    \"Attributes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-put-attributes-request-schema.json
tags:
- AWS
- Cloud Storage
- Data Storage
- Database
- NoSQL
title: PutAttributesRequest
---
