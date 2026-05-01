---
description: GetSchemaResponse schema from Amazon Glue API
layout: schema
name: GetSchemaResponse
properties_list:
- description: ''
  name: RegistryName
  type: object
- description: ''
  name: RegistryArn
  type: object
- description: ''
  name: SchemaName
  type: object
- description: ''
  name: SchemaArn
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: DataFormat
  type: object
- description: ''
  name: Compatibility
  type: object
- description: ''
  name: SchemaCheckpoint
  type: object
- description: ''
  name: LatestSchemaVersion
  type: object
- description: ''
  name: NextSchemaVersion
  type: object
- description: ''
  name: SchemaStatus
  type: object
- description: ''
  name: CreatedTime
  type: object
- description: ''
  name: UpdatedTime
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-schema-response-schema.json
slug: glue-get-schema-response
source_filename: glue-get-schema-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-schema-response-schema.json\",\n  \"title\": \"GetSchemaResponse\",\n  \"description\": \"GetSchemaResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RegistryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaRegistryNameString\"\n        },\n        {\n          \"description\": \"The name of the registry.\"\n        }\n      ]\n    },\n    \"RegistryArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the registry.\"\n        }\n      ]\n    },\n    \"SchemaName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaRegistryNameString\"\n        },\n\
  \        {\n          \"description\": \"The name of the schema.\"\n        }\n      ]\n    },\n    \"SchemaArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the schema.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescriptionString\"\n        },\n        {\n          \"description\": \"A description of schema if specified when created\"\n        }\n      ]\n    },\n    \"DataFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataFormat\"\n        },\n        {\n          \"description\": \"The data format of the schema definition. Currently <code>AVRO</code>, <code>JSON</code> and <code>PROTOBUF</code> are supported.\"\n        }\n      ]\n    },\n    \"Compatibility\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Compatibility\"\
  \n        },\n        {\n          \"description\": \"The compatibility mode of the schema.\"\n        }\n      ]\n    },\n    \"SchemaCheckpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaCheckpointNumber\"\n        },\n        {\n          \"description\": \"The version number of the checkpoint (the last time the compatibility mode was changed).\"\n        }\n      ]\n    },\n    \"LatestSchemaVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionLongNumber\"\n        },\n        {\n          \"description\": \"The latest version of the schema associated with the returned schema definition.\"\n        }\n      ]\n    },\n    \"NextSchemaVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionLongNumber\"\n        },\n        {\n          \"description\": \"The next version of the schema associated with the returned schema definition.\"\n        }\n      ]\n    },\n\
  \    \"SchemaStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaStatus\"\n        },\n        {\n          \"description\": \"The status of the schema.\"\n        }\n      ]\n    },\n    \"CreatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedTimestamp\"\n        },\n        {\n          \"description\": \"The date and time the schema was created.\"\n        }\n      ]\n    },\n    \"UpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdatedTimestamp\"\n        },\n        {\n          \"description\": \"The date and time the schema was updated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-schema-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetSchemaResponse
---
