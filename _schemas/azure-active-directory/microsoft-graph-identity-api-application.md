---
description: Configuration for an application that exposes a web API.
layout: schema
name: ApiApplication
properties_list:
- description: If true, allows an application to use claims mapping without specifying a custom signing key.
  name: acceptMappedClaims
  type: '[''boolean'', ''null'']'
- description: Used for bundling consent. Lists client app IDs that are considered known clients of this API.
  name: knownClientApplications
  type: array
- description: The definition of the delegated permissions exposed by the web API.
  name: oauth2PermissionScopes
  type: array
- description: Lists applications that are pre-authorized with specified delegated permissions.
  name: preAuthorizedApplications
  type: array
- description: The access token version expected by this resource. Possible values are 1 or 2.
  name: requestedAccessTokenVersion
  type: '[''integer'', ''null'']'
provider_name: Azure Active Directory
provider_slug: azure-active-directory
schema_file: json-schema/microsoft-graph-identity-api-application-schema.json
slug: microsoft-graph-identity-api-application
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApiApplication\",\n  \"type\": \"object\",\n  \"description\": \"Configuration for an application that exposes a web API.\",\n  \"properties\": {\n    \"acceptMappedClaims\": {\n      \"type\": \"['boolean', 'null']\",\n      \"description\": \"If true, allows an application to use claims mapping without specifying a custom signing key.\"\n    },\n    \"knownClientApplications\": {\n      \"type\": \"array\",\n      \"description\": \"Used for bundling consent. Lists client app IDs that are considered known clients of this API.\"\n    },\n    \"oauth2PermissionScopes\": {\n      \"type\": \"array\",\n      \"description\": \"The definition of the delegated permissions exposed by the web API.\"\n    },\n    \"preAuthorizedApplications\": {\n      \"type\": \"array\",\n      \"description\": \"Lists applications that are pre-authorized with specified delegated permissions.\"\n    },\n    \"requestedAccessTokenVersion\"\
  : {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"The access token version expected by this resource. Possible values are 1 or 2.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-api-application-schema.json
tags:
- Authentication
- Authorization
- Identity
- Microsoft
- Microsoft Entra
- OAuth
- OpenID Connect
- SAML
- SCIM
- Single Sign-On
- Zero Trust
title: ApiApplication
---
