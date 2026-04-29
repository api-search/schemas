---
description: A Microsoft Entra ID user account managed via Microsoft Graph
layout: schema
name: User
properties_list:
- description: Unique identifier for the user (read-only)
  name: id
  type: string
- description: Name displayed in the address book for the user
  name: displayName
  type: string
- description: Principal name in UPN format (alias@domain)
  name: userPrincipalName
  type: string
- description: Primary SMTP address for the user
  name: mail
  type:
  - string
  - 'null'
- description: Given name (first name) of the user
  name: givenName
  type:
  - string
  - 'null'
- description: Surname (family name or last name) of the user
  name: surname
  type:
  - string
  - 'null'
- description: The user's job title
  name: jobTitle
  type:
  - string
  - 'null'
- description: Department name in which the user works
  name: department
  type:
  - string
  - 'null'
- description: Office location in the user's place of business
  name: officeLocation
  type:
  - string
  - 'null'
- description: Primary cellular telephone number for the user
  name: mobilePhone
  type:
  - string
  - 'null'
- description: Telephone numbers for the user
  name: businessPhones
  type: array
- description: True if the account is enabled; otherwise false
  name: accountEnabled
  type:
  - boolean
  - 'null'
- description: Two-letter country code (ISO 3166) required for license assignment
  name: usageLocation
  type:
  - string
  - 'null'
- description: Preferred language for the user (ISO 639-1 Code, e.g. en-US)
  name: preferredLanguage
  type:
  - string
  - 'null'
- description: Date and time the user was created
  name: createdDateTime
  type:
  - string
  - 'null'
- description: Timestamp of the last password change
  name: lastPasswordChangeDateTime
  type:
  - string
  - 'null'
- description: Password policies enforced for the user
  name: passwordPolicies
  type:
  - string
  - 'null'
- description: Whether the user is a member or guest in the tenant
  name: userType
  type:
  - string
  - 'null'
- description: Licenses assigned to the user
  name: assignedLicenses
  type: array
- description: True if the user is synchronized from on-premises Active Directory
  name: onPremisesSyncEnabled
  type:
  - boolean
  - 'null'
- description: Distinguished name from on-premises Active Directory
  name: onPremisesDistinguishedName
  type:
  - string
  - 'null'
- description: State of a guest/external user invited via Azure AD B2B
  name: externalUserState
  type:
  - string
  - 'null'
provider_name: Microsoft Active Directory
provider_slug: active-directory
schema_file: json-schema/users-user-schema.json
slug: users-user
source_filename: users-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/active-directory/main/json-schema/users-user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"A Microsoft Entra ID user account managed via Microsoft Graph\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the user (read-only)\",\n      \"readOnly\": true\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Name displayed in the address book for the user\",\n      \"maxLength\": 256\n    },\n    \"userPrincipalName\": {\n      \"type\": \"string\",\n      \"description\": \"Principal name in UPN format (alias@domain)\",\n      \"pattern\": \"^[^@]+@[^@]+$\"\n    },\n    \"mail\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"email\",\n      \"description\": \"Primary\
  \ SMTP address for the user\"\n    },\n    \"givenName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Given name (first name) of the user\",\n      \"maxLength\": 64\n    },\n    \"surname\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Surname (family name or last name) of the user\",\n      \"maxLength\": 64\n    },\n    \"jobTitle\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The user's job title\",\n      \"maxLength\": 128\n    },\n    \"department\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Department name in which the user works\",\n      \"maxLength\": 64\n    },\n    \"officeLocation\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Office location in the user's place of business\",\n      \"maxLength\": 128\n    },\n    \"mobilePhone\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Primary cellular telephone number for the user\"\n\
  \    },\n    \"businessPhones\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Telephone numbers for the user\"\n    },\n    \"accountEnabled\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"True if the account is enabled; otherwise false\"\n    },\n    \"usageLocation\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Two-letter country code (ISO 3166) required for license assignment\",\n      \"minLength\": 2,\n      \"maxLength\": 2\n    },\n    \"preferredLanguage\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Preferred language for the user (ISO 639-1 Code, e.g. en-US)\"\n    },\n    \"createdDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the user was created\",\n      \"readOnly\": true\n    },\n    \"lastPasswordChangeDateTime\": {\n      \"type\": [\"string\"\
  , \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last password change\",\n      \"readOnly\": true\n    },\n    \"passwordPolicies\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Password policies enforced for the user\",\n      \"enum\": [\"DisablePasswordExpiration\", \"DisableStrongPassword\", \"DisablePasswordExpiration, DisableStrongPassword\", null]\n    },\n    \"userType\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Whether the user is a member or guest in the tenant\",\n      \"enum\": [\"Member\", \"Guest\", null]\n    },\n    \"assignedLicenses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"skuId\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"disabledPlans\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\",\n\
  \              \"format\": \"uuid\"\n            }\n          }\n        }\n      },\n      \"description\": \"Licenses assigned to the user\"\n    },\n    \"onPremisesSyncEnabled\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"True if the user is synchronized from on-premises Active Directory\",\n      \"readOnly\": true\n    },\n    \"onPremisesDistinguishedName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Distinguished name from on-premises Active Directory\",\n      \"readOnly\": true\n    },\n    \"externalUserState\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"State of a guest/external user invited via Azure AD B2B\",\n      \"enum\": [\"PendingAcceptance\", \"Accepted\", null],\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"displayName\", \"userPrincipalName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/json-schema/users-user-schema.json
tags:
- Active Directory
- Authentication
- Authorization
- Directory Services
- Identity Management
- Microsoft Entra
- Zero Trust
title: User
---
