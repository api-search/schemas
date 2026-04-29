---
description: GetSchemaVersionResponse schema from Amazon Glue API
layout: schema
name: GetSchemaVersionResponse
properties_list:
- description: ''
  name: SchemaVersionId
  type: object
- description: ''
  name: SchemaDefinition
  type: object
- description: ''
  name: DataFormat
  type: object
- description: ''
  name: SchemaArn
  type: object
- description: ''
  name: VersionNumber
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: CreatedTime
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-schema-version-response-schema.json
slug: glue-get-schema-version-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-schema-version-response-schema.json\",\n  \"title\": \"GetSchemaVersionResponse\",\n  \"description\": \"GetSchemaVersionResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SchemaVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaVersionIdString\"\n        },\n        {\n          \"description\": \"The <code>SchemaVersionId</code> of the schema version.\"\n        }\n      ]\n    },\n    \"SchemaDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaDefinitionString\"\n        },\n        {\n          \"description\": \"The schema definition for the schema ID.\"\n        }\n      ]\n    },\n    \"DataFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataFormat\"\
  \n        },\n        {\n          \"description\": \"The data format of the schema definition. Currently <code>AVRO</code>, <code>JSON</code> and <code>PROTOBUF</code> are supported.\"\n        }\n      ]\n    },\n    \"SchemaArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the schema.\"\n        }\n      ]\n    },\n    \"VersionNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionLongNumber\"\n        },\n        {\n          \"description\": \"The version number of the schema.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaVersionStatus\"\n        },\n        {\n          \"description\": \"The status of the schema version. \"\n        }\n      ]\n    },\n    \"CreatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/CreatedTimestamp\"\n        },\n        {\n          \"description\": \"The date and time the schema version was created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-schema-version-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetSchemaVersionResponse
---
