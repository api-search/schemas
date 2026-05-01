---
description: Describes a connection alias association that is used for cross-Region redirection. For more information, see <a href="https://docs.aws.amazon.com/workspaces/latest/adminguide/cross-region-redirection.html"> Cross-Region Redirection for Amazon WorkSpaces</a>.
layout: schema
name: ConnectionAliasAssociation
properties_list:
- description: ''
  name: AssociationStatus
  type: object
- description: ''
  name: AssociatedAccountId
  type: object
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: ConnectionIdentifier
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-connection-alias-association-schema.json
slug: workspaces-connection-alias-association
source_filename: workspaces-connection-alias-association-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AssociationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssociationStatus\"\n        },\n        {\n          \"description\": \"The association status of the connection alias.\"\n        }\n      ]\n    },\n    \"AssociatedAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsAccount\"\n        },\n        {\n          \"description\": \"The identifier of the Amazon Web Services account that associated the connection alias with a directory.\"\n        }\n      ]\n    },\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The identifier of the directory associated with a connection alias.\"\n        }\n      ]\n    },\n    \"ConnectionIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionIdentifier\"\
  \n        },\n        {\n          \"description\": \"The identifier of the connection alias association. You use the connection identifier in the DNS TXT record when you're configuring your DNS routing policies.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes a connection alias association that is used for cross-Region redirection. For more information, see <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/adminguide/cross-region-redirection.html\\\"> Cross-Region Redirection for Amazon WorkSpaces</a>.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConnectionAliasAssociation\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-connection-alias-association-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-connection-alias-association-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ConnectionAliasAssociation
---
