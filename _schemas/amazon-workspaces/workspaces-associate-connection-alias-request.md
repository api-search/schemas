---
description: AssociateConnectionAliasRequest schema from Amazon WorkSpaces API
layout: schema
name: AssociateConnectionAliasRequest
properties_list:
- description: ''
  name: AliasId
  type: object
- description: ''
  name: ResourceId
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-associate-connection-alias-request-schema.json
slug: workspaces-associate-connection-alias-request
source_filename: workspaces-associate-connection-alias-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"AliasId\",\n    \"ResourceId\"\n  ],\n  \"title\": \"AssociateConnectionAliasRequest\",\n  \"properties\": {\n    \"AliasId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionAliasId\"\n        },\n        {\n          \"description\": \"The identifier of the connection alias.\"\n        }\n      ]\n    },\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The identifier of the directory to associate the connection alias with.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-associate-connection-alias-request-schema.json\",\n  \"description\": \"AssociateConnectionAliasRequest schema from Amazon WorkSpaces\
  \ API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-associate-connection-alias-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: AssociateConnectionAliasRequest
---
