---
description: Input to the <code>SetIdentityPoolRoles</code> action.
layout: schema
name: SetIdentityPoolRolesInput
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
schema_file: json-schema/identity-pools-set-identity-pool-roles-input-schema.json
slug: identity-pools-set-identity-pool-roles-input
source_filename: identity-pools-set-identity-pool-roles-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-set-identity-pool-roles-input-schema.json\",\n  \"title\": \"SetIdentityPoolRolesInput\",\n  \"description\": \"Input to the <code>SetIdentityPoolRoles</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolId\"\n        },\n        {\n          \"description\": \"An identity pool ID in the format REGION:GUID.\"\n        }\n      ]\n    },\n    \"Roles\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RolesMap\"\n        },\n        {\n          \"description\": \"The map of roles associated with this pool. For a given role, the key will be either \\\"authenticated\\\" or \\\"unauthenticated\\\" and the value will be the Role ARN.\"\n   \
  \     }\n      ]\n    },\n    \"RoleMappings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleMappingMap\"\n        },\n        {\n          \"description\": \"<p>How users for a specific identity provider are to mapped to roles. This is a string to <a>RoleMapping</a> object map. The string identifies the identity provider, for example, \\\"graph.facebook.com\\\" or \\\"cognito-idp.us-east-1.amazonaws.com/us-east-1_abcdefghi:app_client_id\\\".</p> <p>Up to 25 rules can be specified per identity provider.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityPoolId\",\n    \"Roles\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-set-identity-pool-roles-input-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: SetIdentityPoolRolesInput
---
