---
description: Settings for an application that implements a web API
layout: schema
name: ApiApplication
properties_list:
- description: Allows an application to use claims mapping without specifying a custom signing key
  name: acceptMappedClaims
  type: '[''boolean'', ''null'']'
- description: Used for bundling consent. Lists client app IDs that are considered known clients of this API
  name: knownClientApplications
  type: array
- description: OAuth 2.0 permission scopes exposed by the web API to client applications
  name: oauth2PermissionScopes
  type: array
- description: Lists client applications pre-authorized with specified delegated permissions that do not require user consent
  name: preAuthorizedApplications
  type: array
- description: Specifies the access token version expected by the resource. Possible values are 1 or 2.
  name: requestedAccessTokenVersion
  type: '[''integer'', ''null'']'
provider_name: Microsoft Entra
provider_slug: microsoft-entra
schema_file: json-schema/microsoft-entra-graph-identity-api-application-schema.json
slug: microsoft-entra-graph-identity-api-application
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApiApplication\",\n  \"type\": \"object\",\n  \"description\": \"Settings for an application that implements a web API\",\n  \"properties\": {\n    \"acceptMappedClaims\": {\n      \"type\": \"['boolean', 'null']\",\n      \"description\": \"Allows an application to use claims mapping without specifying a custom signing key\"\n    },\n    \"knownClientApplications\": {\n      \"type\": \"array\",\n      \"description\": \"Used for bundling consent. Lists client app IDs that are considered known clients of this API\"\n    },\n    \"oauth2PermissionScopes\": {\n      \"type\": \"array\",\n      \"description\": \"OAuth 2.0 permission scopes exposed by the web API to client applications\"\n    },\n    \"preAuthorizedApplications\": {\n      \"type\": \"array\",\n      \"description\": \"Lists client applications pre-authorized with specified delegated permissions that do not require user consent\"\
  \n    },\n    \"requestedAccessTokenVersion\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"Specifies the access token version expected by the resource. Possible values are 1 or 2.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra/refs/heads/main/json-schema/microsoft-entra-graph-identity-api-application-schema.json
tags:
- Access Management
- Authentication
- Azure AD
- Entra
- Identity
- Identity Governance
- Microsoft
- Network Security
- Security
- Zero Trust
title: ApiApplication
---
