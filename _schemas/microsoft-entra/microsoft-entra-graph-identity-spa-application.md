---
description: Single-page application configuration
layout: schema
name: SpaApplication
properties_list:
- description: Redirect URIs for single-page application authentication
  name: redirectUris
  type: array
provider_name: Microsoft Entra
provider_slug: microsoft-entra
schema_file: json-schema/microsoft-entra-graph-identity-spa-application-schema.json
slug: microsoft-entra-graph-identity-spa-application
source_filename: microsoft-entra-graph-identity-spa-application-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SpaApplication\",\n  \"type\": \"object\",\n  \"description\": \"Single-page application configuration\",\n  \"properties\": {\n    \"redirectUris\": {\n      \"type\": \"array\",\n      \"description\": \"Redirect URIs for single-page application authentication\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra/refs/heads/main/json-schema/microsoft-entra-graph-identity-spa-application-schema.json
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
title: SpaApplication
---
