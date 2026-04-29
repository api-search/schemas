---
description: Information about a schema extension.
layout: schema
name: SchemaExtensionInfo
properties_list:
- description: ''
  name: DirectoryId
  type: object
- description: ''
  name: SchemaExtensionId
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: SchemaExtensionStatus
  type: object
- description: ''
  name: SchemaExtensionStatusReason
  type: object
- description: ''
  name: StartDateTime
  type: object
- description: ''
  name: EndDateTime
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-schema-extension-info-schema.json
slug: amazon-directory-service-schema-extension-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-schema-extension-info-schema.json\",\n  \"title\": \"SchemaExtensionInfo\",\n  \"description\": \"Information about a schema extension.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DirectoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The identifier of the directory to which the schema extension is applied.\"\n        }\n      ]\n    },\n    \"SchemaExtensionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaExtensionId\"\n        },\n        {\n          \"description\": \"The identifier of the schema extension.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\":\
  \ \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the schema extension.\"\n        }\n      ]\n    },\n    \"SchemaExtensionStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaExtensionStatus\"\n        },\n        {\n          \"description\": \"The current status of the schema extension.\"\n        }\n      ]\n    },\n    \"SchemaExtensionStatusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaExtensionStatusReason\"\n        },\n        {\n          \"description\": \"The reason for the <code>SchemaExtensionStatus</code>.\"\n        }\n      ]\n    },\n    \"StartDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StartDateTime\"\n        },\n        {\n          \"description\": \"The date and time that the schema extension started being applied to the directory.\"\n        }\n      ]\n    },\n    \"EndDateTime\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndDateTime\"\n        },\n        {\n          \"description\": \"The date and time that the schema extension was completed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-schema-extension-info-schema.json
tags:
- Active Directory
- Authentication
- AWS
- Directory Services
- Identity Management
title: SchemaExtensionInfo
---
