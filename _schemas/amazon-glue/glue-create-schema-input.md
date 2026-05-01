---
description: CreateSchemaInput schema from Amazon Glue API
layout: schema
name: CreateSchemaInput
properties_list:
- description: ''
  name: RegistryId
  type: object
- description: ''
  name: SchemaName
  type: object
- description: ''
  name: DataFormat
  type: object
- description: ''
  name: Compatibility
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: SchemaDefinition
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-create-schema-input-schema.json
slug: glue-create-schema-input
source_filename: glue-create-schema-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-schema-input-schema.json\",\n  \"title\": \"CreateSchemaInput\",\n  \"description\": \"CreateSchemaInput schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RegistryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegistryId\"\n        },\n        {\n          \"description\": \" This is a wrapper shape to contain the registry identity fields. If this is not provided, the default registry will be used. The ARN format for the same will be: <code>arn:aws:glue:us-east-2:&lt;customer id&gt;:registry/default-registry:random-5-letter-id</code>.\"\n        }\n      ]\n    },\n    \"SchemaName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaRegistryNameString\"\n        },\n        {\n          \"description\"\
  : \"Name of the schema to be created of max length of 255, and may only contain letters, numbers, hyphen, underscore, dollar sign, or hash mark. No whitespace.\"\n        }\n      ]\n    },\n    \"DataFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataFormat\"\n        },\n        {\n          \"description\": \"The data format of the schema definition. Currently <code>AVRO</code>, <code>JSON</code> and <code>PROTOBUF</code> are supported.\"\n        }\n      ]\n    },\n    \"Compatibility\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Compatibility\"\n        },\n        {\n          \"description\": \"<p>The compatibility mode of the schema. The possible values are:</p> <ul> <li> <p> <i>NONE</i>: No compatibility mode applies. You can use this choice in development scenarios or if you do not know the compatibility mode that you want to apply to schemas. Any new version added will be accepted without undergoing a\
  \ compatibility check.</p> </li> <li> <p> <i>DISABLED</i>: This compatibility choice prevents versioning for a particular schema. You can use this choice to prevent future versioning of a schema.</p> </li> <li> <p> <i>BACKWARD</i>: This compatibility choice is recommended as it allows data receivers to read both the current and one previous schema version. This means that for instance, a new schema version cannot drop data fields or change the type of these fields, so they can't be read by readers using the previous version.</p> </li> <li> <p> <i>BACKWARD_ALL</i>: This compatibility choice allows data receivers to read both the current and all previous schema versions. You can use this choice when you need to delete fields or add optional fields, and check compatibility against all previous schema versions. </p> </li> <li> <p> <i>FORWARD</i>: This compatibility choice allows data receivers to read both the current and one next schema version, but not necessarily later versions. You can\
  \ use this choice when you need to add fields or delete optional fields, but only check compatibility against the last schema version.</p> </li> <li> <p> <i>FORWARD_ALL</i>: This compatibility choice allows data receivers to read written by producers of any new registered schema. You can use this choice when you need to add fields or delete optional fields, and check compatibility against all previous schema versions.</p> </li> <li> <p> <i>FULL</i>: This compatibility choice allows data receivers to read data written by producers using the previous or next version of the schema, but not necessarily earlier or later versions. You can use this choice when you need to add or remove optional fields, but only check compatibility against the last schema version.</p> </li> <li> <p> <i>FULL_ALL</i>: This compatibility choice allows data receivers to read data written by producers using all previous schema versions. You can use this choice when you need to add or remove optional fields, and check\
  \ compatibility against all previous schema versions.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescriptionString\"\n        },\n        {\n          \"description\": \"An optional description of the schema. If description is not provided, there will not be any automatic default value for this.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"Amazon Web Services tags that contain a key value pair and may be searched by console, command line, or API. If specified, follows the Amazon Web Services tags-on-create pattern.\"\n        }\n      ]\n    },\n    \"SchemaDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaDefinitionString\"\n        },\n        {\n          \"description\": \"The schema definition using\
  \ the <code>DataFormat</code> setting for <code>SchemaName</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SchemaName\",\n    \"DataFormat\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-schema-input-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CreateSchemaInput
---
