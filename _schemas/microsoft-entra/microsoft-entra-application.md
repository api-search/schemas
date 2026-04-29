---
description: Schema for a Microsoft Entra ID application registration as represented in the Microsoft Graph API. Defines the application's identity configuration, credentials, permissions, redirect URIs, and sign-in settings.
layout: schema
name: Microsoft Entra Application
properties_list:
- description: Unique identifier for the application object (GUID). This is the directory object ID, not the appId/client ID.
  name: id
  type: string
- description: The unique application (client) identifier assigned by Microsoft Entra ID during app registration.
  name: appId
  type: string
- description: The display name for the application.
  name: displayName
  type: string
- description: Free text field to provide a description of the application object to end users.
  name: description
  type:
  - string
  - 'null'
- description: Specifies which Microsoft accounts are supported for the current application.
  name: signInAudience
  type: string
- description: User-defined URIs that uniquely identify a Web application within its Microsoft Entra tenant or verified custom domain (e.g., api://contoso.com/myapp).
  name: identifierUris
  type: array
- description: ''
  name: web
  type: object
- description: ''
  name: spa
  type: object
- description: ''
  name: publicClient
  type: object
- description: ''
  name: api
  type: object
- description: Specifies the resources that the application needs access to and the set of OAuth permission scopes and app roles required under each resource.
  name: requiredResourceAccess
  type: array
- description: Collection of roles defined for the application. These roles can be assigned to users, groups, or service principals.
  name: appRoles
  type: array
- description: Collection of key (certificate) credentials associated with the application for token signing and verification.
  name: keyCredentials
  type: array
- description: Collection of password credentials (client secrets) associated with the application.
  name: passwordCredentials
  type: array
- description: ''
  name: optionalClaims
  type: object
- description: ''
  name: info
  type: object
- description: Custom strings that can be used to categorize and identify the application.
  name: tags
  type: array
- description: Configures the groups claim issued in user or OAuth 2.0 access tokens.
  name: groupMembershipClaims
  type:
  - string
  - 'null'
- description: Specifies the fallback application type as public client (e.g., installed application on a mobile device). Default is false.
  name: isFallbackPublicClient
  type:
  - boolean
  - 'null'
- description: The default redirect URI. If specified, it is used when no specific redirect URI is matched.
  name: defaultRedirectUri
  type:
  - string
  - 'null'
- description: Publisher certification status of the application.
  name: certification
  type:
  - object
  - 'null'
- description: The verified publisher domain for the application.
  name: publisherDomain
  type: string
- description: The date and time the application was registered.
  name: createdDateTime
  type: string
- description: The date and time the application was deleted.
  name: deletedDateTime
  type:
  - string
  - 'null'
provider_name: Microsoft Entra
provider_slug: microsoft-entra
schema_file: json-schema/microsoft-entra-application-schema.json
slug: microsoft-entra-application
source_filename: microsoft-entra-application-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://graph.microsoft.com/schemas/microsoft-entra/application.json\",\n  \"title\": \"Microsoft Entra Application\",\n  \"description\": \"Schema for a Microsoft Entra ID application registration as represented in the Microsoft Graph API. Defines the application's identity configuration, credentials, permissions, redirect URIs, and sign-in settings.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"displayName\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the application object (GUID). This is the directory object ID, not the appId/client ID.\",\n      \"readOnly\": true\n    },\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique application (client) identifier assigned by Microsoft Entra ID during app registration.\",\n      \"readOnly\": true\n    },\n    \"displayName\": {\n    \
  \  \"type\": \"string\",\n      \"description\": \"The display name for the application.\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Free text field to provide a description of the application object to end users.\",\n      \"maxLength\": 1024\n    },\n    \"signInAudience\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies which Microsoft accounts are supported for the current application.\",\n      \"enum\": [\n        \"AzureADMyOrg\",\n        \"AzureADMultipleOrgs\",\n        \"AzureADandPersonalMicrosoftAccount\",\n        \"PersonalMicrosoftAccount\"\n      ],\n      \"default\": \"AzureADMyOrg\"\n    },\n    \"identifierUris\": {\n      \"type\": \"array\",\n      \"description\": \"User-defined URIs that uniquely identify a Web application within its Microsoft Entra tenant or verified custom domain (e.g., api://contoso.com/myapp).\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\"\
  : \"uri\"\n      }\n    },\n    \"web\": {\n      \"$ref\": \"#/$defs/WebApplication\"\n    },\n    \"spa\": {\n      \"$ref\": \"#/$defs/SpaApplication\"\n    },\n    \"publicClient\": {\n      \"$ref\": \"#/$defs/PublicClientApplication\"\n    },\n    \"api\": {\n      \"$ref\": \"#/$defs/ApiApplication\"\n    },\n    \"requiredResourceAccess\": {\n      \"type\": \"array\",\n      \"description\": \"Specifies the resources that the application needs access to and the set of OAuth permission scopes and app roles required under each resource.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/RequiredResourceAccess\"\n      }\n    },\n    \"appRoles\": {\n      \"type\": \"array\",\n      \"description\": \"Collection of roles defined for the application. These roles can be assigned to users, groups, or service principals.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AppRole\"\n      }\n    },\n    \"keyCredentials\": {\n      \"type\": \"array\",\n      \"description\": \"Collection\
  \ of key (certificate) credentials associated with the application for token signing and verification.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/KeyCredential\"\n      }\n    },\n    \"passwordCredentials\": {\n      \"type\": \"array\",\n      \"description\": \"Collection of password credentials (client secrets) associated with the application.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PasswordCredential\"\n      }\n    },\n    \"optionalClaims\": {\n      \"$ref\": \"#/$defs/OptionalClaims\"\n    },\n    \"info\": {\n      \"$ref\": \"#/$defs/InformationalUrl\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Custom strings that can be used to categorize and identify the application.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"groupMembershipClaims\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Configures the groups claim issued in user or OAuth 2.0 access tokens.\",\n      \"\
  enum\": [\n        \"None\",\n        \"SecurityGroup\",\n        \"DirectoryRole\",\n        \"ApplicationGroup\",\n        \"All\",\n        null\n      ]\n    },\n    \"isFallbackPublicClient\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Specifies the fallback application type as public client (e.g., installed application on a mobile device). Default is false.\",\n      \"default\": false\n    },\n    \"defaultRedirectUri\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The default redirect URI. If specified, it is used when no specific redirect URI is matched.\"\n    },\n    \"certification\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Publisher certification status of the application.\",\n      \"readOnly\": true,\n      \"properties\": {\n        \"isPublisherAttested\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the application has been attested by the publisher.\"\n      \
  \  },\n        \"isCertifiedByMicrosoft\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the application has been certified by Microsoft.\"\n        },\n        \"lastCertificationDateTime\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp of last certification.\"\n        }\n      }\n    },\n    \"publisherDomain\": {\n      \"type\": \"string\",\n      \"description\": \"The verified publisher domain for the application.\",\n      \"readOnly\": true\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the application was registered.\",\n      \"readOnly\": true\n    },\n    \"deletedDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the application was deleted.\",\n      \"readOnly\": true\n    }\n  },\n  \"$defs\"\
  : {\n    \"WebApplication\": {\n      \"type\": \"object\",\n      \"description\": \"Settings for a web application including redirect URIs and implicit grant configuration.\",\n      \"properties\": {\n        \"redirectUris\": {\n          \"type\": \"array\",\n          \"description\": \"Specifies URLs to which Azure AD will redirect after authentication for web applications.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          }\n        },\n        \"homePageUrl\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Home page or landing page URL of the application.\",\n          \"format\": \"uri\"\n        },\n        \"logoutUrl\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"URL used by the authorization service to sign out the user using front-channel, back-channel, or SAML logout protocols.\",\n          \"format\": \"uri\"\n        },\n        \"implicitGrantSettings\"\
  : {\n          \"type\": \"object\",\n          \"description\": \"Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.\",\n          \"properties\": {\n            \"enableIdTokenIssuance\": {\n              \"type\": \"boolean\",\n              \"description\": \"Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.\",\n              \"default\": false\n            },\n            \"enableAccessTokenIssuance\": {\n              \"type\": \"boolean\",\n              \"description\": \"Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.\",\n              \"default\": false\n            }\n          }\n        }\n      }\n    },\n    \"SpaApplication\": {\n      \"type\": \"object\",\n      \"description\": \"Settings for a single-page application including redirect URIs for MSAL.js 2.0 auth code flow with PKCE.\",\n      \"properties\": {\n        \"redirectUris\"\
  : {\n          \"type\": \"array\",\n          \"description\": \"Specifies redirect URIs for the SPA to receive authorization codes and access tokens.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          }\n        }\n      }\n    },\n    \"PublicClientApplication\": {\n      \"type\": \"object\",\n      \"description\": \"Settings for installed (public client) applications on mobile and desktop devices.\",\n      \"properties\": {\n        \"redirectUris\": {\n          \"type\": \"array\",\n          \"description\": \"Specifies redirect URIs for native/public client applications (mobile and desktop).\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"ApiApplication\": {\n      \"type\": \"object\",\n      \"description\": \"Settings for an application that implements a web API including permission scopes and pre-authorized applications.\",\n      \"properties\": {\n      \
  \  \"acceptMappedClaims\": {\n          \"type\": [\"boolean\", \"null\"],\n          \"description\": \"When true, allows an application to use claims mapping without specifying a custom signing key.\"\n        },\n        \"knownClientApplications\": {\n          \"type\": \"array\",\n          \"description\": \"Client application IDs considered as known clients for bundling consent.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          }\n        },\n        \"oauth2PermissionScopes\": {\n          \"type\": \"array\",\n          \"description\": \"The definition of the delegated permissions (OAuth 2.0 scopes) exposed by the web API.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/PermissionScope\"\n          }\n        },\n        \"preAuthorizedApplications\": {\n          \"type\": \"array\",\n          \"description\": \"Lists applications pre-authorized with the specified delegated permissions to access this API\
  \ without user consent.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"appId\": {\n                \"type\": \"string\",\n                \"description\": \"The appId of the pre-authorized client application.\"\n              },\n              \"delegatedPermissionIds\": {\n                \"type\": \"array\",\n                \"description\": \"The IDs of the OAuth 2.0 permission scopes the client is pre-authorized for.\",\n                \"items\": {\n                  \"type\": \"string\",\n                  \"format\": \"uuid\"\n                }\n              }\n            }\n          }\n        },\n        \"requestedAccessTokenVersion\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Specifies the access token version expected by this resource. Values: 1 (v1.0 tokens) or 2 (v2.0 tokens).\",\n          \"enum\": [1, 2, null]\n        }\n      }\n    },\n    \"PermissionScope\": {\n \
  \     \"type\": \"object\",\n      \"description\": \"Defines a delegated permission (OAuth 2.0 scope) that a web API application exposes to client applications.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique delegated permission identifier inside the collection of scopes.\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The scope value string included in OAuth 2.0 access tokens (e.g., User.Read, Mail.Send).\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Whether this scope can be consented by end users or only by admins.\",\n          \"enum\": [\"User\", \"Admin\"]\n        },\n        \"adminConsentDisplayName\": {\n          \"type\": \"string\",\n          \"description\": \"Title of the permission shown on the admin consent page.\"\n        },\n        \"adminConsentDescription\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Description of the permission shown on the admin consent page.\"\n        },\n        \"userConsentDisplayName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Title of the permission shown on the user consent page.\"\n        },\n        \"userConsentDescription\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Description of the permission shown on the user consent page.\"\n        },\n        \"isEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"When creating or updating a permission, this must be set to true. To delete a permission, first set to false.\",\n          \"default\": true\n        }\n      }\n    },\n    \"RequiredResourceAccess\": {\n      \"type\": \"object\",\n      \"description\": \"Specifies the set of OAuth 2.0 permission scopes and app roles under a specified resource that an application requires.\",\n      \"\
  properties\": {\n        \"resourceAppId\": {\n          \"type\": \"string\",\n          \"description\": \"The appId of the resource application (e.g., 00000003-0000-0000-c000-000000000000 for Microsoft Graph).\"\n        },\n        \"resourceAccess\": {\n          \"type\": \"array\",\n          \"description\": \"The list of OAuth 2.0 permission scopes and app roles required from the specified resource.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"format\": \"uuid\",\n                \"description\": \"The unique identifier for an app role or OAuth2 permission scope exposed by the resource application.\"\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"description\": \"Specifies whether the id references a delegated permission (Scope) or an application permission (Role).\",\n                \"enum\"\
  : [\"Scope\", \"Role\"]\n              }\n            },\n            \"required\": [\"id\", \"type\"]\n          }\n        }\n      },\n      \"required\": [\"resourceAppId\", \"resourceAccess\"]\n    },\n    \"AppRole\": {\n      \"type\": \"object\",\n      \"description\": \"Represents an application role that can be requested by a client application calling another app, or assigned to users or groups.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique role identifier inside the appRoles collection.\"\n        },\n        \"allowedMemberTypes\": {\n          \"type\": \"array\",\n          \"description\": \"Specifies whether the app role can be assigned to users/groups, applications, or both.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\"User\", \"Application\"]\n          }\n        },\n        \"displayName\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Display name for the permission that appears in the app role assignment and consent experiences.\"\n        },\n        \"description\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Description of the permission that appears in admin app assignment and consent experiences.\"\n        },\n        \"value\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Value included in the roles claim in ID tokens and access tokens authenticating an assigned user or service principal.\",\n          \"maxLength\": 120\n        },\n        \"isEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"When creating or updating an app role, this must be set to true.\",\n          \"default\": true\n        },\n        \"origin\": {\n          \"type\": \"string\",\n          \"description\": \"Specifies if the app role is defined on the application or service principal object.\",\n          \"\
  readOnly\": true\n        }\n      }\n    },\n    \"KeyCredential\": {\n      \"type\": \"object\",\n      \"description\": \"Contains a key (certificate) credential associated with an application used for token signing and verification.\",\n      \"properties\": {\n        \"keyId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier for the key.\"\n        },\n        \"displayName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Friendly name for the key.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of key credential.\",\n          \"enum\": [\"AsymmetricX509Cert\", \"X509CertAndPassword\"]\n        },\n        \"usage\": {\n          \"type\": \"string\",\n          \"description\": \"A string that describes the purpose for which the key can be used.\",\n          \"enum\": [\"Sign\", \"Verify\"]\n        },\n        \"key\"\
  : {\n          \"type\": \"string\",\n          \"contentEncoding\": \"base64\",\n          \"description\": \"The certificate's raw data in byte array converted to Base64 string.\"\n        },\n        \"startDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time at which the credential becomes valid.\"\n        },\n        \"endDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time at which the credential expires.\"\n        },\n        \"customKeyIdentifier\": {\n          \"type\": [\"string\", \"null\"],\n          \"contentEncoding\": \"base64\",\n          \"description\": \"Custom key identifier (typically the certificate thumbprint).\"\n        }\n      }\n    },\n    \"PasswordCredential\": {\n      \"type\": \"object\",\n      \"description\": \"Represents a password credential (client secret) associated with an application.\"\
  ,\n      \"properties\": {\n        \"keyId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier for the password.\",\n          \"readOnly\": true\n        },\n        \"displayName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Friendly name for the password. Maximum length is 32 characters.\",\n          \"maxLength\": 32\n        },\n        \"hint\": {\n          \"type\": \"string\",\n          \"description\": \"Contains the first three characters of the password.\",\n          \"readOnly\": true,\n          \"maxLength\": 3\n        },\n        \"secretText\": {\n          \"type\": \"string\",\n          \"description\": \"The strong password or secret generated by Microsoft Entra ID. Only returned at creation time and cannot be retrieved later.\",\n          \"readOnly\": true\n        },\n        \"startDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"\
  date-time\",\n          \"description\": \"The date and time at which the password becomes valid.\"\n        },\n        \"endDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time at which the password expires.\"\n        }\n      }\n    },\n    \"OptionalClaims\": {\n      \"type\": \"object\",\n      \"description\": \"Declares the optional claims requested by an application. The application can configure optional claims to be returned in tokens from the Microsoft identity platform.\",\n      \"properties\": {\n        \"idToken\": {\n          \"type\": \"array\",\n          \"description\": \"The optional claims requested in the JWT ID token.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/OptionalClaim\"\n          }\n        },\n        \"accessToken\": {\n          \"type\": \"array\",\n          \"description\": \"The optional claims requested in the JWT access token.\",\n          \"items\"\
  : {\n            \"$ref\": \"#/$defs/OptionalClaim\"\n          }\n        },\n        \"saml2Token\": {\n          \"type\": \"array\",\n          \"description\": \"The optional claims requested in the SAML token.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/OptionalClaim\"\n          }\n        }\n      }\n    },\n    \"OptionalClaim\": {\n      \"type\": \"object\",\n      \"description\": \"An optional claim associated with an application.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the optional claim.\"\n        },\n        \"source\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The source (directory object) of the claim. If null, the claim is a predefined optional claim.\"\n        },\n        \"essential\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, the claim specified by the client is necessary to ensure a smooth authorization\
  \ experience.\",\n          \"default\": false\n        },\n        \"additionalProperties\": {\n          \"type\": \"array\",\n          \"description\": \"Additional properties of the claim.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"InformationalUrl\": {\n      \"type\": \"object\",\n      \"description\": \"Basic profile information of the application for user-facing scenarios.\",\n      \"properties\": {\n        \"logoUrl\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"CDN URL to the application's logo.\",\n          \"format\": \"uri\"\n        },\n        \"marketingUrl\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Link to the application's marketing page.\",\n          \"format\": \"uri\"\n        },\n        \"privacyStatementUrl\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Link to the application's privacy statement.\"\
  ,\n          \"format\": \"uri\"\n        },\n        \"supportUrl\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Link to the application's support page.\",\n          \"format\": \"uri\"\n        },\n        \"termsOfServiceUrl\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Link to the application's terms of service statement.\",\n          \"format\": \"uri\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra/refs/heads/main/json-schema/microsoft-entra-application-schema.json
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
title: Microsoft Entra Application
---
