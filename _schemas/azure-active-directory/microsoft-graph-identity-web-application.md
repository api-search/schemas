---
description: Configuration for a web application.
layout: schema
name: WebApplication
properties_list:
- description: Home page or landing page of the application.
  name: homePageUrl
  type: '[''string'', ''null'']'
- description: URL used by the authorization service to sign out a user.
  name: logoutUrl
  type: '[''string'', ''null'']'
- description: URIs to which Azure AD will redirect after authentication.
  name: redirectUris
  type: array
- description: ''
  name: implicitGrantSettings
  type: object
provider_name: Azure Active Directory
provider_slug: azure-active-directory
schema_file: json-schema/microsoft-graph-identity-web-application-schema.json
slug: microsoft-graph-identity-web-application
source_filename: microsoft-graph-identity-web-application-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WebApplication\",\n  \"type\": \"object\",\n  \"description\": \"Configuration for a web application.\",\n  \"properties\": {\n    \"homePageUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Home page or landing page of the application.\"\n    },\n    \"logoutUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"URL used by the authorization service to sign out a user.\"\n    },\n    \"redirectUris\": {\n      \"type\": \"array\",\n      \"description\": \"URIs to which Azure AD will redirect after authentication.\"\n    },\n    \"implicitGrantSettings\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-web-application-schema.json
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
title: WebApplication
---
