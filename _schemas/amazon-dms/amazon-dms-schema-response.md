---
description: Describes a schema in a Fleet Advisor collector inventory.
layout: schema
name: SchemaResponse
properties_list:
- description: ''
  name: CodeLineCount
  type: object
- description: ''
  name: CodeSize
  type: object
- description: ''
  name: Complexity
  type: object
- description: ''
  name: Server
  type: object
- description: ''
  name: DatabaseInstance
  type: object
- description: ''
  name: SchemaId
  type: object
- description: ''
  name: SchemaName
  type: object
- description: ''
  name: OriginalSchema
  type: object
- description: ''
  name: Similarity
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-schema-response-schema.json
slug: amazon-dms-schema-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-schema-response-schema.json\",\n  \"title\": \"SchemaResponse\",\n  \"description\": \"Describes a schema in a Fleet Advisor collector inventory.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CodeLineCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongOptional\"\n        },\n        {\n          \"description\": \"The number of lines of code in a schema in a Fleet Advisor collector inventory.\"\n        }\n      ]\n    },\n    \"CodeSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongOptional\"\n        },\n        {\n          \"description\": \"The size level of the code in a schema in a Fleet Advisor collector inventory.\"\n        }\n      ]\n    },\n    \"Complexity\": {\n      \"allOf\": [\n        {\n    \
  \      \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The complexity level of the code in a schema in a Fleet Advisor collector inventory.\"\n        }\n      ]\n    },\n    \"Server\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServerShortInfoResponse\"\n        },\n        {\n          \"description\": \"The database server for a schema in a Fleet Advisor collector inventory.\"\n        }\n      ]\n    },\n    \"DatabaseInstance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatabaseShortInfoResponse\"\n        },\n        {\n          \"description\": \"The database for a schema in a Fleet Advisor collector inventory.\"\n        }\n      ]\n    },\n    \"SchemaId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ID of a schema in a Fleet Advisor collector inventory.\"\n     \
  \   }\n      ]\n    },\n    \"SchemaName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of a schema in a Fleet Advisor collector inventory.\"\n        }\n      ]\n    },\n    \"OriginalSchema\": {\n      \"$ref\": \"#/components/schemas/SchemaShortInfoResponse\"\n    },\n    \"Similarity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DoubleOptional\"\n        },\n        {\n          \"description\": \"The similarity value for a schema in a Fleet Advisor collector inventory. A higher similarity value indicates that a schema is likely to be a duplicate.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-schema-response-schema.json
tags:
- AWS
- Data Replication
- Database
- Database Migration
- Migration
title: SchemaResponse
---
