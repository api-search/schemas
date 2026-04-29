---
description: Represents an application registration in Microsoft Entra ID. Defines the app's identity configuration, credentials, permissions requested, and reply URLs.
layout: schema
name: Application
properties_list:
- description: Unique identifier for the application object (GUID). This is the object ID, not the appId.
  name: id
  type: string
- description: The unique application identifier assigned by Microsoft Entra ID (also known as the client ID)
  name: appId
  type: string
- description: The display name for the application
  name: displayName
  type: string
- description: An optional description of the application
  name: description
  type: '[''string'', ''null'']'
- description: Specifies which Microsoft accounts are supported for the application
  name: signInAudience
  type: string
- description: URIs that uniquely identify the application within its Azure AD tenant or verified custom domain
  name: identifierUris
  type: array
- description: Specifies the resources that the application needs access to and the set of OAuth permission scopes and app roles needed under each resource
  name: requiredResourceAccess
  type: array
- description: Collection of roles defined for the application that can be assigned to users, groups, or service principals
  name: appRoles
  type: array
- description: Collection of certificate credentials associated with the app
  name: keyCredentials
  type: array
- description: Collection of password credentials (client secrets)
  name: passwordCredentials
  type: array
- description: Public client settings for mobile and desktop apps
  name: publicClient
  type: object
- description: Custom strings used to categorize and identify the application
  name: tags
  type: array
- description: The date and time the application was registered
  name: createdDateTime
  type: string
provider_name: Microsoft Entra
provider_slug: microsoft-entra
schema_file: json-schema/microsoft-entra-graph-identity-application-schema.json
slug: microsoft-entra-graph-identity-application
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Application\",\n  \"type\": \"object\",\n  \"description\": \"Represents an application registration in Microsoft Entra ID. Defines the app's identity configuration, credentials, permissions requested, and reply URLs.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the application object (GUID). This is the object ID, not the appId.\"\n    },\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique application identifier assigned by Microsoft Entra ID (also known as the client ID)\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name for the application\"\n    },\n    \"description\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"An optional description of the application\"\n    },\n    \"signInAudience\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Specifies which Microsoft accounts are supported for the application\"\n    },\n    \"identifierUris\": {\n      \"type\": \"array\",\n      \"description\": \"URIs that uniquely identify the application within its Azure AD tenant or verified custom domain\"\n    },\n    \"requiredResourceAccess\": {\n      \"type\": \"array\",\n      \"description\": \"Specifies the resources that the application needs access to and the set of OAuth permission scopes and app roles needed under each resource\"\n    },\n    \"appRoles\": {\n      \"type\": \"array\",\n      \"description\": \"Collection of roles defined for the application that can be assigned to users, groups, or service principals\"\n    },\n    \"keyCredentials\": {\n      \"type\": \"array\",\n      \"description\": \"Collection of certificate credentials associated with the app\"\n    },\n    \"passwordCredentials\": {\n      \"type\": \"array\",\n      \"description\": \"Collection of password\
  \ credentials (client secrets)\"\n    },\n    \"publicClient\": {\n      \"type\": \"object\",\n      \"description\": \"Public client settings for mobile and desktop apps\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Custom strings used to categorize and identify the application\"\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the application was registered\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra/refs/heads/main/json-schema/microsoft-entra-graph-identity-application-schema.json
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
title: Application
---
