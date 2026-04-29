---
description: DisassociateConnectionAliasRequest schema from Amazon WorkSpaces API
layout: schema
name: DisassociateConnectionAliasRequest
properties_list:
- description: ''
  name: AliasId
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-disassociate-connection-alias-request-schema.json
slug: workspaces-disassociate-connection-alias-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"AliasId\"\n  ],\n  \"title\": \"DisassociateConnectionAliasRequest\",\n  \"properties\": {\n    \"AliasId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionAliasId\"\n        },\n        {\n          \"description\": \"The identifier of the connection alias to disassociate.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-disassociate-connection-alias-request-schema.json\",\n  \"description\": \"DisassociateConnectionAliasRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-disassociate-connection-alias-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DisassociateConnectionAliasRequest
---
