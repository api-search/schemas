---
description: Represents a license assigned to a user.
layout: schema
name: AssignedLicense
properties_list:
- description: A collection of the unique identifiers for plans that have been disabled.
  name: disabledPlans
  type: array
- description: The unique identifier for the SKU.
  name: skuId
  type: string
provider_name: Microsoft Azure Active Directory
provider_slug: microsoft-azure-active-directory
schema_file: json-schema/microsoft-graph-identity-assigned-license-schema.json
slug: microsoft-graph-identity-assigned-license
source_filename: microsoft-graph-identity-assigned-license-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssignedLicense\",\n  \"type\": \"object\",\n  \"description\": \"Represents a license assigned to a user.\",\n  \"properties\": {\n    \"disabledPlans\": {\n      \"type\": \"array\",\n      \"description\": \"A collection of the unique identifiers for plans that have been disabled.\"\n    },\n    \"skuId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the SKU.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-assigned-license-schema.json
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
title: AssignedLicense
---
