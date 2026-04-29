---
description: CreateConnectionAliasRequest schema from Amazon WorkSpaces API
layout: schema
name: CreateConnectionAliasRequest
properties_list:
- description: ''
  name: ConnectionString
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-create-connection-alias-request-schema.json
slug: workspaces-create-connection-alias-request
source_filename: workspaces-create-connection-alias-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ConnectionString\"\n  ],\n  \"title\": \"CreateConnectionAliasRequest\",\n  \"properties\": {\n    \"ConnectionString\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionString\"\n        },\n        {\n          \"description\": \"<p>A connection string in the form of a fully qualified domain name (FQDN), such as <code>www.example.com</code>.</p> <important> <p>After you create a connection string, it is always associated to your Amazon Web Services account. You cannot recreate the same connection string with a different account, even if you delete all instances of it from the original account. The connection string is globally reserved for your account.</p> </important>\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The tags to associate with the\
  \ connection alias.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-connection-alias-request-schema.json\",\n  \"description\": \"CreateConnectionAliasRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-connection-alias-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: CreateConnectionAliasRequest
---
