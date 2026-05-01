---
description: AssociateConnectionAliasResult schema from Amazon WorkSpaces API
layout: schema
name: AssociateConnectionAliasResult
properties_list:
- description: ''
  name: ConnectionIdentifier
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-associate-connection-alias-result-schema.json
slug: workspaces-associate-connection-alias-result
source_filename: workspaces-associate-connection-alias-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConnectionIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionIdentifier\"\n        },\n        {\n          \"description\": \"The identifier of the connection alias association. You use the connection identifier in the DNS TXT record when you're configuring your DNS routing policies. \"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssociateConnectionAliasResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-associate-connection-alias-result-schema.json\",\n  \"description\": \"AssociateConnectionAliasResult schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-associate-connection-alias-result-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: AssociateConnectionAliasResult
---
