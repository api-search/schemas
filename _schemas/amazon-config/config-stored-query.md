---
description: Provides the details of a stored query.
layout: schema
name: StoredQuery
properties_list:
- description: ''
  name: QueryId
  type: object
- description: ''
  name: QueryArn
  type: object
- description: ''
  name: QueryName
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Expression
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-stored-query-schema.json
slug: config-stored-query
source_filename: config-stored-query-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-stored-query-schema.json\",\n  \"title\": \"StoredQuery\",\n  \"description\": \"Provides the details of a stored query.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"QueryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryId\"\n        },\n        {\n          \"description\": \"The ID of the query.\"\n        }\n      ]\n    },\n    \"QueryArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryArn\"\n        },\n        {\n          \"description\": \"Amazon Resource Name (ARN) of the query. For example, arn:partition:service:region:account-id:resource-type/resource-name/resource-id.\"\n        }\n      ]\n    },\n    \"QueryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryName\"\
  \n        },\n        {\n          \"description\": \"The name of the query.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryDescription\"\n        },\n        {\n          \"description\": \"A unique description for the query.\"\n        }\n      ]\n    },\n    \"Expression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryExpression\"\n        },\n        {\n          \"description\": \"The expression of the query. For example, <code>SELECT resourceId, resourceType, supplementaryConfiguration.BucketVersioningConfiguration.status WHERE resourceType = 'AWS::S3::Bucket' AND supplementaryConfiguration.BucketVersioningConfiguration.status = 'Off'.</code> \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"QueryName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-stored-query-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: StoredQuery
---
