---
description: Returned in response to a successful <code>GetIdentityPoolRoles</code> operation.
layout: schema
name: GetIdentityPoolRolesResponse
properties_list:
- description: ''
  name: IdentityPoolId
  type: object
- description: ''
  name: Roles
  type: object
- description: ''
  name: RoleMappings
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/identity-pools-get-identity-pool-roles-response-schema.json
slug: identity-pools-get-identity-pool-roles-response
source_filename: identity-pools-get-identity-pool-roles-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-get-identity-pool-roles-response-schema.json\",\n  \"title\": \"GetIdentityPoolRolesResponse\",\n  \"description\": \"Returned in response to a successful <code>GetIdentityPoolRoles</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolId\"\n        },\n        {\n          \"description\": \"An identity pool ID in the format REGION:GUID.\"\n        }\n      ]\n    },\n    \"Roles\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RolesMap\"\n        },\n        {\n          \"description\": \"The map of roles associated with this pool. Currently only authenticated and unauthenticated roles are supported.\"\n        }\n      ]\n    },\n\
  \    \"RoleMappings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleMappingMap\"\n        },\n        {\n          \"description\": \"How users for a specific identity provider are to mapped to roles. This is a String-to-<a>RoleMapping</a> object map. The string identifies the identity provider, for example, \\\"graph.facebook.com\\\" or \\\"cognito-idp.us-east-1.amazonaws.com/us-east-1_abcdefghi:app_client_id\\\".\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-get-identity-pool-roles-response-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: GetIdentityPoolRolesResponse
---
