---
description: UpdateConnectionAliasPermissionRequest schema from Amazon WorkSpaces API
layout: schema
name: UpdateConnectionAliasPermissionRequest
properties_list:
- description: ''
  name: AliasId
  type: object
- description: ''
  name: ConnectionAliasPermission
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-update-connection-alias-permission-request-schema.json
slug: workspaces-update-connection-alias-permission-request
source_filename: workspaces-update-connection-alias-permission-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"AliasId\",\n    \"ConnectionAliasPermission\"\n  ],\n  \"title\": \"UpdateConnectionAliasPermissionRequest\",\n  \"properties\": {\n    \"AliasId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionAliasId\"\n        },\n        {\n          \"description\": \"The identifier of the connection alias that you want to update permissions for.\"\n        }\n      ]\n    },\n    \"ConnectionAliasPermission\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionAliasPermission\"\n        },\n        {\n          \"description\": \"Indicates whether to share or unshare the connection alias with the specified Amazon Web Services account.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-update-connection-alias-permission-request-schema.json\"\
  ,\n  \"description\": \"UpdateConnectionAliasPermissionRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-update-connection-alias-permission-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: UpdateConnectionAliasPermissionRequest
---
