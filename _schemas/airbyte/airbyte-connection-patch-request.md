---
description: ConnectionPatchRequest schema from Airbyte API
layout: schema
name: ConnectionPatchRequest
properties_list:
- description: Optional name of the connection
  name: name
  type: string
- description: ''
  name: configurations
  type: object
- description: ''
  name: schedule
  type: object
- description: ''
  name: dataResidency
  type: string
- description: ''
  name: namespaceDefinition
  type: object
- description: Used when namespaceDefinition is 'custom_format'. If blank then behaves like namespaceDefinition = 'destination'. If "${SOURCE_NAMESPACE}" then behaves like namespaceDefinition = 'source'.
  name: namespaceFormat
  type: string
- description: Prefix that will be prepended to the name of each stream when it is written to the destination (ex. “airbyte_” causes “projects” => “airbyte_projects”).
  name: prefix
  type: string
- description: ''
  name: nonBreakingSchemaUpdatesBehavior
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: tags
  type: array
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-connection-patch-request-schema.json
slug: airbyte-connection-patch-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-connection-patch-request-schema.json\",\n  \"title\": \"ConnectionPatchRequest\",\n  \"description\": \"ConnectionPatchRequest schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"Optional name of the connection\",\n      \"type\": \"string\"\n    },\n    \"configurations\": {\n      \"$ref\": \"#/components/schemas/StreamConfigurations\"\n    },\n    \"schedule\": {\n      \"$ref\": \"#/components/schemas/AirbyteApiConnectionSchedule\"\n    },\n    \"dataResidency\": {\n      \"deprecated\": true,\n      \"x-speakeasy-deprecation-message\": \"We no longer support modifying dataResidency on Community and Enterprise connections. All connections will use the dataResidency of their associated workspace.\",\n      \"type\": \"string\"\n    },\n\
  \    \"namespaceDefinition\": {\n      \"$ref\": \"#/components/schemas/NamespaceDefinitionEnumNoDefault\"\n    },\n    \"namespaceFormat\": {\n      \"type\": \"string\",\n      \"description\": \"Used when namespaceDefinition is 'custom_format'. If blank then behaves like namespaceDefinition = 'destination'. If \\\"${SOURCE_NAMESPACE}\\\" then behaves like namespaceDefinition = 'source'.\",\n      \"default\": null,\n      \"example\": \"${SOURCE_NAMESPACE}\"\n    },\n    \"prefix\": {\n      \"type\": \"string\",\n      \"description\": \"Prefix that will be prepended to the name of each stream when it is written to the destination (ex. \\u201cairbyte_\\u201d causes \\u201cprojects\\u201d => \\u201cairbyte_projects\\u201d).\"\n    },\n    \"nonBreakingSchemaUpdatesBehavior\": {\n      \"$ref\": \"#/components/schemas/NonBreakingSchemaUpdatesBehaviorEnumNoDefault\"\n    },\n    \"status\": {\n      \"$ref\": \"#/components/schemas/ConnectionStatusEnum\"\n    },\n    \"tags\": {\n   \
  \   \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tag\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-connection-patch-request-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: ConnectionPatchRequest
---
