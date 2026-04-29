---
description: Representation of a pipeline template input parameter.
layout: schema
name: InputDescriptor
properties_list:
- description: Description of the input parameter.
  name: description
  type: string
- description: Identifier of the input parameter.
  name: id
  type: string
- description: List of possible values for the input parameter.
  name: possibleValues
  type: array
- description: Data type of the value of the input parameter.
  name: type
  type: string
provider_name: Azure DevOps
provider_slug: azure-dev-ops
schema_file: json-schema/azure-dev-ops-input-descriptor-schema.json
slug: azure-dev-ops-input-descriptor
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-input-descriptor-schema.json\",\n  \"title\": \"InputDescriptor\",\n  \"description\": \"Representation of a pipeline template input parameter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"Description of the input parameter.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"Identifier of the input parameter.\",\n      \"type\": \"string\"\n    },\n    \"possibleValues\": {\n      \"description\": \"List of possible values for the input parameter.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/InputValue\"\n      },\n      \"type\": \"array\"\n    },\n    \"type\": {\n      \"description\": \"Data type of the value of the input parameter.\",\n      \"enum\": [\n        \"String\",\n        \"SecureString\"\
  ,\n        \"Int\",\n        \"Bool\",\n        \"Authorization\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"InputDataType\"\n      }\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-input-descriptor-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
title: InputDescriptor
---
