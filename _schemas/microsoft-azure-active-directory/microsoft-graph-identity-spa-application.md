---
description: Configuration for a single-page application.
layout: schema
name: SpaApplication
properties_list:
- description: Redirect URIs for the single-page application using authorization code flow with PKCE.
  name: redirectUris
  type: array
provider_name: Microsoft Azure Active Directory
provider_slug: microsoft-azure-active-directory
schema_file: json-schema/microsoft-graph-identity-spa-application-schema.json
slug: microsoft-graph-identity-spa-application
source_filename: microsoft-graph-identity-spa-application-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SpaApplication\",\n  \"type\": \"object\",\n  \"description\": \"Configuration for a single-page application.\",\n  \"properties\": {\n    \"redirectUris\": {\n      \"type\": \"array\",\n      \"description\": \"Redirect URIs for the single-page application using authorization code flow with PKCE.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-spa-application-schema.json
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
title: SpaApplication
---
