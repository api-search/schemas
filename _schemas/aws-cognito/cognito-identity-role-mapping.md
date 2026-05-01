---
description: A role mapping.
layout: schema
name: RoleMapping
properties_list:
- description: ''
  name: Type
  type: object
- description: ''
  name: AmbiguousRoleResolution
  type: object
- description: ''
  name: RulesConfiguration
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-role-mapping-schema.json
slug: cognito-identity-role-mapping
source_filename: cognito-identity-role-mapping-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleMappingType\"\n        },\n        {\n          \"description\": \"The role mapping type. Token will use <code>cognito:roles</code> and <code>cognito:preferred_role</code> claims from the Cognito identity provider token to map groups to roles. Rules will attempt to match claims from the token to map to a role.\"\n        }\n      ]\n    },\n    \"AmbiguousRoleResolution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmbiguousRoleResolutionType\"\n        },\n        {\n          \"description\": \"<p>If you specify Token or Rules as the <code>Type</code>, <code>AmbiguousRoleResolution</code> is required.</p> <p>Specifies the action to be taken if either no rules match the claim value for the <code>Rules</code> type, or there is no <code>cognito:preferred_role</code> claim and there are multiple <code>cognito:roles</code>\
  \ matches for the <code>Token</code> type.</p>\"\n        }\n      ]\n    },\n    \"RulesConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RulesConfigurationType\"\n        },\n        {\n          \"description\": \"<p>The rules to be used for mapping users to roles.</p> <p>If you specify Rules as the role mapping type, <code>RulesConfiguration</code> is required.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Type\"\n  ],\n  \"description\": \"A role mapping.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-role-mapping-schema.json\",\n  \"title\": \"RoleMapping\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-role-mapping-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: RoleMapping
---
