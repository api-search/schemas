---
description: Represents an instance of an application in a directory. A service principal is the local representation or application instance of a global application object in a single tenant. It defines what the app can do in the tenant, who can access it, and what resources the app can access.
layout: schema
name: ServicePrincipal
properties_list:
- description: True if the service principal account is enabled.
  name: accountEnabled
  type: boolean
- description: Description copied from the associated application.
  name: appDescription
  type: '[''string'', ''null'']'
- description: The display name exposed by the associated application.
  name: appDisplayName
  type: '[''string'', ''null'']'
- description: The unique identifier for the associated application (its appId property). Required on creation.
  name: appId
  type: string
- description: Contains the tenant ID where the application is registered.
  name: appOwnerOrganizationId
  type: '[''string'', ''null'']'
- description: Specifies whether users or other service principals need to be granted an app role assignment before accessing.
  name: appRoleAssignmentRequired
  type: boolean
- description: Roles exposed by the associated application.
  name: appRoles
  type: array
- description: The display name for the service principal.
  name: displayName
  type: string
- description: Home page or landing page of the application.
  name: homepage
  type: '[''string'', ''null'']'
- description: ''
  name: keyCredentials
  type: array
- description: URL for the authentication provider to redirect users to for sign-in.
  name: loginUrl
  type: '[''string'', ''null'']'
- description: ''
  name: logoutUrl
  type: '[''string'', ''null'']'
- description: Email addresses where Azure AD sends notifications when the active certificate is near expiration.
  name: notificationEmailAddresses
  type: array
- description: The delegated permissions exposed by the application.
  name: oauth2PermissionScopes
  type: array
- description: ''
  name: passwordCredentials
  type: array
- description: The URLs that user tokens are sent to for sign-in, or the redirect URIs for authorization code and access token responses.
  name: replyUrls
  type: array
- description: Contains the list of identifierUris and the appId from the associated application.
  name: servicePrincipalNames
  type: array
- description: Identifies whether the service principal represents an Application, ManagedIdentity, Legacy, or SocialIdp.
  name: servicePrincipalType
  type: string
- description: The audience that can sign in.
  name: signInAudience
  type: string
- description: Custom strings used to categorize the service principal. The WindowsAzureActiveDirectoryIntegratedApp tag is used by the portal.
  name: tags
  type: array
- description: ''
  name: tokenEncryptionKeyId
  type: '[''string'', ''null'']'
provider_name: Microsoft Azure Active Directory
provider_slug: microsoft-azure-active-directory
schema_file: json-schema/microsoft-graph-identity-service-principal-schema.json
slug: microsoft-graph-identity-service-principal
source_filename: microsoft-graph-identity-service-principal-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServicePrincipal\",\n  \"type\": \"object\",\n  \"description\": \"Represents an instance of an application in a directory. A service principal is the local representation or application instance of a global application object in a single tenant. It defines what the app can do in the tenant, who can access it, and what resources the app can access.\",\n  \"properties\": {\n    \"accountEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the service principal account is enabled.\"\n    },\n    \"appDescription\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Description copied from the associated application.\"\n    },\n    \"appDisplayName\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The display name exposed by the associated application.\"\n    },\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The unique identifier for the associated application (its appId property). Required on creation.\"\n    },\n    \"appOwnerOrganizationId\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Contains the tenant ID where the application is registered.\"\n    },\n    \"appRoleAssignmentRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether users or other service principals need to be granted an app role assignment before accessing.\"\n    },\n    \"appRoles\": {\n      \"type\": \"array\",\n      \"description\": \"Roles exposed by the associated application.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name for the service principal.\"\n    },\n    \"homepage\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Home page or landing page of the application.\"\n    },\n    \"keyCredentials\": {\n      \"type\": \"array\"\n    },\n    \"loginUrl\": {\n      \"type\"\
  : \"['string', 'null']\",\n      \"description\": \"URL for the authentication provider to redirect users to for sign-in.\"\n    },\n    \"logoutUrl\": {\n      \"type\": \"['string', 'null']\"\n    },\n    \"notificationEmailAddresses\": {\n      \"type\": \"array\",\n      \"description\": \"Email addresses where Azure AD sends notifications when the active certificate is near expiration.\"\n    },\n    \"oauth2PermissionScopes\": {\n      \"type\": \"array\",\n      \"description\": \"The delegated permissions exposed by the application.\"\n    },\n    \"passwordCredentials\": {\n      \"type\": \"array\"\n    },\n    \"replyUrls\": {\n      \"type\": \"array\",\n      \"description\": \"The URLs that user tokens are sent to for sign-in, or the redirect URIs for authorization code and access token responses.\"\n    },\n    \"servicePrincipalNames\": {\n      \"type\": \"array\",\n      \"description\": \"Contains the list of identifierUris and the appId from the associated application.\"\
  \n    },\n    \"servicePrincipalType\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies whether the service principal represents an Application, ManagedIdentity, Legacy, or SocialIdp.\"\n    },\n    \"signInAudience\": {\n      \"type\": \"string\",\n      \"description\": \"The audience that can sign in.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Custom strings used to categorize the service principal. The WindowsAzureActiveDirectoryIntegratedApp tag is used by the portal.\"\n    },\n    \"tokenEncryptionKeyId\": {\n      \"type\": \"['string', 'null']\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-service-principal-schema.json
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
title: ServicePrincipal
---
