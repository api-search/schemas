---
description: Represents an Azure Active Directory directory object. This is the base type for most directory resources.
layout: schema
name: DirectoryObject
properties_list:
- description: The OData type of the directory object.
  name: '@odata.type'
  type: string
- description: The unique identifier for the object. Globally unique across all directory objects.
  name: id
  type: string
- description: Date and time when this object was deleted.
  name: deletedDateTime
  type: string
provider_name: Azure Active Directory
provider_slug: azure-active-directory
schema_file: json-schema/microsoft-graph-identity-directory-object-schema.json
slug: microsoft-graph-identity-directory-object
source_filename: microsoft-graph-identity-directory-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DirectoryObject\",\n  \"type\": \"object\",\n  \"description\": \"Represents an Azure Active Directory directory object. This is the base type for most directory resources.\",\n  \"properties\": {\n    \"@odata.type\": {\n      \"type\": \"string\",\n      \"description\": \"The OData type of the directory object.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the object. Globally unique across all directory objects.\"\n    },\n    \"deletedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when this object was deleted.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-directory-object-schema.json
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
title: DirectoryObject
---
