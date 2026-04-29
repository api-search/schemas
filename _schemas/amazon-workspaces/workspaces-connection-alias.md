---
description: Describes a connection alias. Connection aliases are used for cross-Region redirection. For more information, see <a href="https://docs.aws.amazon.com/workspaces/latest/adminguide/cross-region-redirection.html"> Cross-Region Redirection for Amazon WorkSpaces</a>.
layout: schema
name: ConnectionAlias
properties_list:
- description: ''
  name: ConnectionString
  type: object
- description: ''
  name: AliasId
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: OwnerAccountId
  type: object
- description: ''
  name: Associations
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-connection-alias-schema.json
slug: workspaces-connection-alias
source_filename: workspaces-connection-alias-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConnectionString\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionString\"\n        },\n        {\n          \"description\": \"The connection string specified for the connection alias. The connection string must be in the form of a fully qualified domain name (FQDN), such as <code>www.example.com</code>.\"\n        }\n      ]\n    },\n    \"AliasId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionAliasId\"\n        },\n        {\n          \"description\": \"The identifier of the connection alias.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionAliasState\"\n        },\n        {\n          \"description\": \"The current state of the connection alias.\"\n        }\n      ]\n    },\n    \"OwnerAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/AwsAccount\"\n        },\n        {\n          \"description\": \"The identifier of the Amazon Web Services account that owns the connection alias.\"\n        }\n      ]\n    },\n    \"Associations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionAliasAssociationList\"\n        },\n        {\n          \"description\": \"The association status of the connection alias.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes a connection alias. Connection aliases are used for cross-Region redirection. For more information, see <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/adminguide/cross-region-redirection.html\\\"> Cross-Region Redirection for Amazon WorkSpaces</a>.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConnectionAlias\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-connection-alias-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-connection-alias-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ConnectionAlias
---
