---
description: A Microsoft Entra application registration managed via Microsoft Graph
layout: schema
name: Application
properties_list:
- description: Unique identifier for the application object (not the client ID)
  name: id
  type: string
- description: The application (client) ID used in OAuth2 flows
  name: appId
  type: string
- description: Display name of the application
  name: displayName
  type: string
- description: Free text description for the application
  name: description
  type:
  - string
  - 'null'
- description: Microsoft account types supported by the application
  name: signInAudience
  type: string
- description: URIs that identify the application within the tenant
  name: identifierUris
  type: array
- description: Web platform configuration for the application
  name: web
  type: object
- description: API permissions required by the application
  name: requiredResourceAccess
  type: array
- description: Certificate credentials for the application
  name: keyCredentials
  type: array
- description: Client secret credential metadata (secret value only returned at creation)
  name: passwordCredentials
  type: array
- description: ''
  name: createdDateTime
  type:
  - string
  - 'null'
- description: ''
  name: deletedDateTime
  type:
  - string
  - 'null'
provider_name: Microsoft Active Directory
provider_slug: active-directory
schema_file: json-schema/applications-application-schema.json
slug: applications-application
source_filename: applications-application-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/active-directory/main/json-schema/applications-application-schema.json\",\n  \"title\": \"Application\",\n  \"description\": \"A Microsoft Entra application registration managed via Microsoft Graph\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the application object (not the client ID)\",\n      \"readOnly\": true\n    },\n    \"appId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The application (client) ID used in OAuth2 flows\",\n      \"readOnly\": true\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the application\",\n      \"maxLength\": 256\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"\
  description\": \"Free text description for the application\"\n    },\n    \"signInAudience\": {\n      \"type\": \"string\",\n      \"description\": \"Microsoft account types supported by the application\",\n      \"enum\": [\n        \"AzureADMyOrg\",\n        \"AzureADMultipleOrgs\",\n        \"AzureADandPersonalMicrosoftAccount\",\n        \"PersonalMicrosoftAccount\"\n      ]\n    },\n    \"identifierUris\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      },\n      \"description\": \"URIs that identify the application within the tenant\"\n    },\n    \"web\": {\n      \"type\": \"object\",\n      \"description\": \"Web platform configuration for the application\",\n      \"properties\": {\n        \"redirectUris\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          }\n        },\n        \"logoutUrl\": {\n          \"type\": [\"\
  string\", \"null\"],\n          \"format\": \"uri\"\n        },\n        \"implicitGrantSettings\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"enableAccessTokenIssuance\": {\n              \"type\": \"boolean\"\n            },\n            \"enableIdTokenIssuance\": {\n              \"type\": \"boolean\"\n            }\n          }\n        }\n      }\n    },\n    \"requiredResourceAccess\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"resourceAppId\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"resourceAccess\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"id\": {\n                  \"type\": \"string\",\n                  \"format\": \"uuid\"\n                },\n                \"type\": {\n                  \"type\"\
  : \"string\",\n                  \"enum\": [\"Role\", \"Scope\"]\n                }\n              }\n            }\n          }\n        }\n      },\n      \"description\": \"API permissions required by the application\"\n    },\n    \"keyCredentials\": {\n      \"type\": \"array\",\n      \"description\": \"Certificate credentials for the application\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"keyId\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"type\": {\n            \"type\": \"string\"\n          },\n          \"usage\": {\n            \"type\": \"string\",\n            \"enum\": [\"Sign\", \"Verify\"]\n          },\n          \"displayName\": {\n            \"type\": \"string\"\n          },\n          \"startDateTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"endDateTime\": {\n            \"type\": \"string\",\n  \
  \          \"format\": \"date-time\"\n          }\n        }\n      }\n    },\n    \"passwordCredentials\": {\n      \"type\": \"array\",\n      \"description\": \"Client secret credential metadata (secret value only returned at creation)\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"keyId\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"displayName\": {\n            \"type\": \"string\"\n          },\n          \"startDateTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"endDateTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"hint\": {\n            \"type\": \"string\",\n            \"description\": \"First three characters of the application secret\"\n          }\n        }\n      }\n    },\n    \"createdDateTime\": {\n      \"type\": [\"string\", \"null\"],\n    \
  \  \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"deletedDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"displayName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/json-schema/applications-application-schema.json
tags:
- Active Directory
- Authentication
- Authorization
- Directory Services
- Identity Management
- Microsoft Entra
- Zero Trust
title: Application
---
