---
description: JSON Schema for configuring a GraphQL schema stitching gateway, defining subschemas, type merging, and field delegation.
layout: schema
name: Schema Stitching Configuration
properties_list:
- description: Array of subschemas to stitch together into a unified gateway schema.
  name: subschemas
  type: array
- description: Additional GraphQL type definitions to extend the stitched schema with extra fields or types.
  name: typeDefs
  type: string
- description: Additional resolver functions for types and fields added via typeDefs.
  name: resolvers
  type: object
- description: Whether to automatically merge types with the same name across subschemas.
  name: mergeTypes
  type: boolean
provider_name: Schema Stitching
provider_slug: schema-stitching
schema_file: json-schema/schema-stitching-config-schema.json
slug: schema-stitching-config
source_filename: schema-stitching-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://schema-stitching.dev/schema-stitching-config-schema.json\",\n  \"title\": \"Schema Stitching Configuration\",\n  \"description\": \"JSON Schema for configuring a GraphQL schema stitching gateway, defining subschemas, type merging, and field delegation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subschemas\": {\n      \"type\": \"array\",\n      \"description\": \"Array of subschemas to stitch together into a unified gateway schema.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/SubschemaConfig\"\n      }\n    },\n    \"typeDefs\": {\n      \"type\": \"string\",\n      \"description\": \"Additional GraphQL type definitions to extend the stitched schema with extra fields or types.\"\n    },\n    \"resolvers\": {\n      \"type\": \"object\",\n      \"description\": \"Additional resolver functions for types and fields added via typeDefs.\",\n      \"additionalProperties\"\
  : true\n    },\n    \"mergeTypes\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Whether to automatically merge types with the same name across subschemas.\"\n    }\n  },\n  \"definitions\": {\n    \"SubschemaConfig\": {\n      \"type\": \"object\",\n      \"required\": [\"schema\"],\n      \"properties\": {\n        \"schema\": {\n          \"type\": \"string\",\n          \"description\": \"The GraphQL schema SDL string or reference to a remote schema.\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the remote GraphQL service endpoint.\"\n        },\n        \"batch\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Whether to batch queries to this subschema using DataLoader-style batching.\"\n        },\n        \"merge\": {\n          \"type\": \"object\",\n          \"description\": \"Type merging configuration\
  \ for this subschema.\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/definitions/MergeTypeConfig\"\n          }\n        },\n        \"transforms\": {\n          \"type\": \"array\",\n          \"description\": \"Schema transforms to apply to this subschema before stitching.\",\n          \"items\": {\n            \"$ref\": \"#/definitions/SchemaTransform\"\n          }\n        },\n        \"executor\": {\n          \"type\": \"string\",\n          \"description\": \"Custom executor function name for this subschema.\"\n        }\n      }\n    },\n    \"MergeTypeConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"selectionSet\": {\n          \"type\": \"string\",\n          \"description\": \"GraphQL selection set for fetching the key fields required to merge this type.\",\n          \"example\": \"{ id }\"\n        },\n        \"fieldName\": {\n          \"type\": \"string\",\n          \"description\": \"The query field name used to fetch\
  \ a single merged type by key.\"\n        },\n        \"argsFromKeys\": {\n          \"type\": \"string\",\n          \"description\": \"Function expression mapping key values to query arguments.\"\n        },\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"Function expression extracting the merge key from a type object.\"\n        },\n        \"dataLoaderOptions\": {\n          \"type\": \"object\",\n          \"description\": \"DataLoader configuration for batched type merging.\",\n          \"properties\": {\n            \"maxBatchSize\": {\n              \"type\": \"integer\",\n              \"description\": \"Maximum number of keys per batch request.\"\n            }\n          }\n        }\n      }\n    },\n    \"SchemaTransform\": {\n      \"type\": \"object\",\n      \"description\": \"A schema transformation to apply to a subschema.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n    \
  \        \"FilterRootFields\",\n            \"FilterObjectFields\",\n            \"RenameTypes\",\n            \"RenameRootFields\",\n            \"RenameObjectFields\",\n            \"WrapQuery\",\n            \"HoistField\",\n            \"PruneSchema\"\n          ],\n          \"description\": \"The type of transformation to apply.\"\n        },\n        \"config\": {\n          \"type\": \"object\",\n          \"description\": \"Configuration specific to the transform type.\",\n          \"additionalProperties\": true\n        }\n      }\n    },\n    \"StitchingDirectivesConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for stitching directives SDL approach.\",\n      \"properties\": {\n        \"keyDirective\": {\n          \"type\": \"string\",\n          \"default\": \"key\",\n          \"description\": \"Name of the directive used to specify merge keys.\"\n        },\n        \"mergeDirective\": {\n          \"type\": \"string\",\n          \"default\"\
  : \"merge\",\n          \"description\": \"Name of the directive used to configure type merging.\"\n        },\n        \"computedDirective\": {\n          \"type\": \"string\",\n          \"default\": \"computed\",\n          \"description\": \"Name of the directive used to specify computed fields.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-stitching/refs/heads/main/json-schema/schema-stitching-config-schema.json
tags:
- API Composition
- API Gateway
- Federation
- GraphQL
- Microservices
- Schema Stitching
- Type Merging
title: Schema Stitching Configuration
---
