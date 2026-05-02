---
description: Configuration for a public client (mobile/desktop) application.
layout: schema
name: PublicClientApplication
properties_list:
- description: Redirect URIs for the public client application.
  name: redirectUris
  type: array
provider_name: Microsoft Azure Active Directory
provider_slug: microsoft-azure-active-directory
schema_file: json-schema/microsoft-graph-identity-public-client-application-schema.json
slug: microsoft-graph-identity-public-client-application
source_filename: microsoft-graph-identity-public-client-application-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PublicClientApplication\",\n  \"type\": \"object\",\n  \"description\": \"Configuration for a public client (mobile/desktop) application.\",\n  \"properties\": {\n    \"redirectUris\": {\n      \"type\": \"array\",\n      \"description\": \"Redirect URIs for the public client application.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-public-client-application-schema.json
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
title: PublicClientApplication
---
