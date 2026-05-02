---
description: Represents an application registration in Azure AD. An application object is the global definition of an application, specifying how tokens are issued, the resources the application needs to access, and the actions it can perform.
layout: schema
name: Application
properties_list:
- description: The unique identifier assigned by Azure AD when the app is registered. Also known as the client ID.
  name: appId
  type: string
- description: The display name for the application.
  name: displayName
  type: string
- description: A free text field to describe the application.
  name: description
  type: '[''string'', ''null'']'
- description: The date and time the application was registered.
  name: createdDateTime
  type: string
- description: URIs that identify the application within its Azure AD tenant. Also known as App ID URIs.
  name: identifierUris
  type: array
- description: The collection of key credentials (certificates) associated with the application.
  name: keyCredentials
  type: array
- description: The collection of password credentials (client secrets) associated with the application.
  name: passwordCredentials
  type: array
- description: The collection of roles defined for the application.
  name: appRoles
  type: array
- description: Specifies the resources that the application needs access to.
  name: requiredResourceAccess
  type: array
- description: Specifies the Microsoft accounts supported for the current application.
  name: signInAudience
  type: string
- description: Custom strings that can be used to categorize the application.
  name: tags
  type: array
- description: The verified publisher domain for the application.
  name: publisherDomain
  type: string
provider_name: Microsoft Azure Active Directory
provider_slug: microsoft-azure-active-directory
schema_file: json-schema/microsoft-graph-identity-application-schema.json
slug: microsoft-graph-identity-application
source_filename: microsoft-graph-identity-application-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Application\",\n  \"type\": \"object\",\n  \"description\": \"Represents an application registration in Azure AD. An application object is the global definition of an application, specifying how tokens are issued, the resources the application needs to access, and the actions it can perform.\",\n  \"properties\": {\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier assigned by Azure AD when the app is registered. Also known as the client ID.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name for the application.\"\n    },\n    \"description\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"A free text field to describe the application.\"\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the application was registered.\"\
  \n    },\n    \"identifierUris\": {\n      \"type\": \"array\",\n      \"description\": \"URIs that identify the application within its Azure AD tenant. Also known as App ID URIs.\"\n    },\n    \"keyCredentials\": {\n      \"type\": \"array\",\n      \"description\": \"The collection of key credentials (certificates) associated with the application.\"\n    },\n    \"passwordCredentials\": {\n      \"type\": \"array\",\n      \"description\": \"The collection of password credentials (client secrets) associated with the application.\"\n    },\n    \"appRoles\": {\n      \"type\": \"array\",\n      \"description\": \"The collection of roles defined for the application.\"\n    },\n    \"requiredResourceAccess\": {\n      \"type\": \"array\",\n      \"description\": \"Specifies the resources that the application needs access to.\"\n    },\n    \"signInAudience\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the Microsoft accounts supported for the current application.\"\
  \n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Custom strings that can be used to categorize the application.\"\n    },\n    \"publisherDomain\": {\n      \"type\": \"string\",\n      \"description\": \"The verified publisher domain for the application.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-application-schema.json
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
title: Application
---
