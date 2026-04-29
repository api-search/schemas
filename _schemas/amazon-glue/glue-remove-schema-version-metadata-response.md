---
description: RemoveSchemaVersionMetadataResponse schema from Amazon Glue API
layout: schema
name: RemoveSchemaVersionMetadataResponse
properties_list:
- description: ''
  name: SchemaArn
  type: object
- description: ''
  name: SchemaName
  type: object
- description: ''
  name: RegistryName
  type: object
- description: ''
  name: LatestVersion
  type: object
- description: ''
  name: VersionNumber
  type: object
- description: ''
  name: SchemaVersionId
  type: object
- description: ''
  name: MetadataKey
  type: object
- description: ''
  name: MetadataValue
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-remove-schema-version-metadata-response-schema.json
slug: glue-remove-schema-version-metadata-response
source_filename: glue-remove-schema-version-metadata-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-remove-schema-version-metadata-response-schema.json\",\n  \"title\": \"RemoveSchemaVersionMetadataResponse\",\n  \"description\": \"RemoveSchemaVersionMetadataResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SchemaArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the schema.\"\n        }\n      ]\n    },\n    \"SchemaName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaRegistryNameString\"\n        },\n        {\n          \"description\": \"The name of the schema.\"\n        }\n      ]\n    },\n    \"RegistryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaRegistryNameString\"\
  \n        },\n        {\n          \"description\": \"The name of the registry.\"\n        }\n      ]\n    },\n    \"LatestVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LatestSchemaVersionBoolean\"\n        },\n        {\n          \"description\": \"The latest version of the schema.\"\n        }\n      ]\n    },\n    \"VersionNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionLongNumber\"\n        },\n        {\n          \"description\": \"The version number of the schema.\"\n        }\n      ]\n    },\n    \"SchemaVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaVersionIdString\"\n        },\n        {\n          \"description\": \"The version ID for the schema version.\"\n        }\n      ]\n    },\n    \"MetadataKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetadataKeyString\"\n        },\n        {\n          \"\
  description\": \"The metadata key.\"\n        }\n      ]\n    },\n    \"MetadataValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetadataValueString\"\n        },\n        {\n          \"description\": \"The value of the metadata key.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-remove-schema-version-metadata-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: RemoveSchemaVersionMetadataResponse
---
