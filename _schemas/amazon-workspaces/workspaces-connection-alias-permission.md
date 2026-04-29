---
description: Describes the permissions for a connection alias. Connection aliases are used for cross-Region redirection. For more information, see <a href="https://docs.aws.amazon.com/workspaces/latest/adminguide/cross-region-redirection.html"> Cross-Region Redirection for Amazon WorkSpaces</a>.
layout: schema
name: ConnectionAliasPermission
properties_list:
- description: ''
  name: SharedAccountId
  type: object
- description: ''
  name: AllowAssociation
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-connection-alias-permission-schema.json
slug: workspaces-connection-alias-permission
source_filename: workspaces-connection-alias-permission-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"SharedAccountId\",\n    \"AllowAssociation\"\n  ],\n  \"properties\": {\n    \"SharedAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsAccount\"\n        },\n        {\n          \"description\": \"The identifier of the Amazon Web Services account that the connection alias is shared with.\"\n        }\n      ]\n    },\n    \"AllowAssociation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"Indicates whether the specified Amazon Web Services account is allowed to associate the connection alias with a directory.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes the permissions for a connection alias. Connection aliases are used for cross-Region redirection. For more information, see <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/adminguide/cross-region-redirection.html\\\
  \"> Cross-Region Redirection for Amazon WorkSpaces</a>.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConnectionAliasPermission\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-connection-alias-permission-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-connection-alias-permission-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ConnectionAliasPermission
---
