---
description: A Microsoft Entra service principal — the local tenant instance of an application
layout: schema
name: ServicePrincipal
properties_list:
- description: Unique identifier for the service principal object
  name: id
  type: string
- description: Application (client) ID of the associated application registration
  name: appId
  type: string
- description: Display name for the service principal
  name: displayName
  type: string
- description: Type of service principal
  name: servicePrincipalType
  type: string
- description: True if the service principal account is enabled
  name: accountEnabled
  type:
  - boolean
  - 'null'
- description: Application roles exposed by the associated application
  name: appRoles
  type: array
- description: Delegated permission scopes exposed by the application
  name: oauth2PermissionScopes
  type: array
- description: Home page or landing page of the application
  name: homepage
  type:
  - string
  - 'null'
- description: URL to direct users for sign-in (for SP-initiated SAML SSO)
  name: loginUrl
  type:
  - string
  - 'null'
- description: URLs where tokens are sent after authentication
  name: replyUrls
  type: array
- description: Strings that categorize the application
  name: tags
  type: array
- description: ''
  name: createdDateTime
  type:
  - string
  - 'null'
provider_name: Microsoft Active Directory
provider_slug: active-directory
schema_file: json-schema/applications-service-principal-schema.json
slug: applications-service-principal
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/active-directory/main/json-schema/applications-service-principal-schema.json\",\n  \"title\": \"ServicePrincipal\",\n  \"description\": \"A Microsoft Entra service principal — the local tenant instance of an application\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the service principal object\",\n      \"readOnly\": true\n    },\n    \"appId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Application (client) ID of the associated application registration\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the service principal\"\n    },\n    \"servicePrincipalType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of\
  \ service principal\",\n      \"enum\": [\"Application\", \"Legacy\", \"ManagedIdentity\", \"SocialIdp\"]\n    },\n    \"accountEnabled\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"True if the service principal account is enabled\"\n    },\n    \"appRoles\": {\n      \"type\": \"array\",\n      \"description\": \"Application roles exposed by the associated application\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"displayName\": {\n            \"type\": \"string\"\n          },\n          \"description\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          },\n          \"allowedMemberTypes\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\",\n              \"enum\": [\"User\", \"Application\"]\n\
  \            }\n          },\n          \"isEnabled\": {\n            \"type\": \"boolean\"\n          }\n        }\n      }\n    },\n    \"oauth2PermissionScopes\": {\n      \"type\": \"array\",\n      \"description\": \"Delegated permission scopes exposed by the application\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"adminConsentDisplayName\": {\n            \"type\": \"string\"\n          },\n          \"adminConsentDescription\": {\n            \"type\": \"string\"\n          },\n          \"userConsentDisplayName\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\"User\", \"Admin\"]\n          },\n          \"isEnabled\": {\n            \"type\": \"boolean\"\n          }\n  \
  \      }\n      }\n    },\n    \"homepage\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"Home page or landing page of the application\"\n    },\n    \"loginUrl\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"URL to direct users for sign-in (for SP-initiated SAML SSO)\"\n    },\n    \"replyUrls\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      },\n      \"description\": \"URLs where tokens are sent after authentication\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Strings that categorize the application\"\n    },\n    \"createdDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/json-schema/applications-service-principal-schema.json
tags:
- Active Directory
- Authentication
- Authorization
- Directory Services
- Identity Management
- Microsoft Entra
- Zero Trust
title: ServicePrincipal
---
