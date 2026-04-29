---
description: Represents a Microsoft Entra ID user account. Contains identity, contact, organizational, and authentication properties.
layout: schema
name: User
properties_list:
- description: Unique identifier for the user (GUID). Assigned automatically by the directory.
  name: id
  type: string
- description: The name displayed in the address book for the user
  name: displayName
  type: string
- description: The given name (first name) of the user
  name: givenName
  type: '[''string'', ''null'']'
- description: The surname (family name) of the user
  name: surname
  type: '[''string'', ''null'']'
- description: The SMTP address of the user. This property cannot be set during creation for cloud-only users.
  name: mail
  type: '[''string'', ''null'']'
- description: The user principal name (UPN) of the user in the format alias@domain. The domain must be present in the tenant's verified domains collection.
  name: userPrincipalName
  type: string
- description: The mail alias for the user. Must be specified when creating a new user.
  name: mailNickname
  type: string
- description: true if the account is enabled; otherwise, false. Must be specified when creating a new user.
  name: accountEnabled
  type: boolean
- description: The user's job title
  name: jobTitle
  type: '[''string'', ''null'']'
- description: The department in which the user works
  name: department
  type: '[''string'', ''null'']'
- description: The office location in the user's place of business
  name: officeLocation
  type: '[''string'', ''null'']'
- description: The company name associated with the user
  name: companyName
  type: '[''string'', ''null'']'
- description: The primary cellular telephone number for the user
  name: mobilePhone
  type: '[''string'', ''null'']'
- description: The telephone numbers for the user's business
  name: businessPhones
  type: array
- description: The street address of the user's place of business
  name: streetAddress
  type: '[''string'', ''null'']'
- description: The city in which the user is located
  name: city
  type: '[''string'', ''null'']'
- description: The state or province in the user's address
  name: state
  type: '[''string'', ''null'']'
- description: The postal code for the user's postal address
  name: postalCode
  type: '[''string'', ''null'']'
- description: The country or region in which the user is located (ISO 3166 two-letter code)
  name: country
  type: '[''string'', ''null'']'
- description: Two-letter country code (ISO 3166). Required for users assigned licenses due to legal requirements for checking service availability.
  name: usageLocation
  type: '[''string'', ''null'']'
- description: The preferred language for the user in ISO 639-1 code format (e.g., en-US)
  name: preferredLanguage
  type: '[''string'', ''null'']'
- description: Classification of the user type relative to the tenant
  name: userType
  type: string
- description: The employee identifier assigned by the organization
  name: employeeId
  type: '[''string'', ''null'']'
- description: Captures the type of worker (e.g., Employee, Contractor, Consultant, Vendor)
  name: employeeType
  type: '[''string'', ''null'']'
- description: The date and time when the user was hired
  name: employeeHireDate
  type: '[''string'', ''null'']'
- description: true if this user is synced from an on-premises directory; false if originally created in Azure AD; null if never synced
  name: onPremisesSyncEnabled
  type: '[''boolean'', ''null'']'
- description: The on-premises SAM account name synchronized from the on-premises directory
  name: onPremisesSamAccountName
  type: '[''string'', ''null'']'
- description: List of proxy addresses for the user including SMTP and smtp prefixed addresses
  name: proxyAddresses
  type: array
- description: Licenses assigned to the user
  name: assignedLicenses
  type: array
- description: The date and time the user was created
  name: createdDateTime
  type: string
- description: The date and time of the user's most recent interactive sign-in activity
  name: lastSignInDateTime
  type: '[''string'', ''null'']'
provider_name: Microsoft Entra
provider_slug: microsoft-entra
schema_file: json-schema/microsoft-entra-graph-identity-user-schema.json
slug: microsoft-entra-graph-identity-user
source_filename: microsoft-entra-graph-identity-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"User\",\n  \"type\": \"object\",\n  \"description\": \"Represents a Microsoft Entra ID user account. Contains identity, contact, organizational, and authentication properties.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the user (GUID). Assigned automatically by the directory.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The name displayed in the address book for the user\"\n    },\n    \"givenName\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The given name (first name) of the user\"\n    },\n    \"surname\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The surname (family name) of the user\"\n    },\n    \"mail\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The SMTP address of the user. This property cannot\
  \ be set during creation for cloud-only users.\"\n    },\n    \"userPrincipalName\": {\n      \"type\": \"string\",\n      \"description\": \"The user principal name (UPN) of the user in the format alias@domain. The domain must be present in the tenant's verified domains collection.\"\n    },\n    \"mailNickname\": {\n      \"type\": \"string\",\n      \"description\": \"The mail alias for the user. Must be specified when creating a new user.\"\n    },\n    \"accountEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"true if the account is enabled; otherwise, false. Must be specified when creating a new user.\"\n    },\n    \"jobTitle\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The user's job title\"\n    },\n    \"department\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The department in which the user works\"\n    },\n    \"officeLocation\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The\
  \ office location in the user's place of business\"\n    },\n    \"companyName\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The company name associated with the user\"\n    },\n    \"mobilePhone\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The primary cellular telephone number for the user\"\n    },\n    \"businessPhones\": {\n      \"type\": \"array\",\n      \"description\": \"The telephone numbers for the user's business\"\n    },\n    \"streetAddress\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The street address of the user's place of business\"\n    },\n    \"city\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The city in which the user is located\"\n    },\n    \"state\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The state or province in the user's address\"\n    },\n    \"postalCode\": {\n      \"type\": \"['string', 'null']\",\n      \"description\"\
  : \"The postal code for the user's postal address\"\n    },\n    \"country\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The country or region in which the user is located (ISO 3166 two-letter code)\"\n    },\n    \"usageLocation\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Two-letter country code (ISO 3166). Required for users assigned licenses due to legal requirements for checking service availability.\"\n    },\n    \"preferredLanguage\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The preferred language for the user in ISO 639-1 code format (e.g., en-US)\"\n    },\n    \"userType\": {\n      \"type\": \"string\",\n      \"description\": \"Classification of the user type relative to the tenant\"\n    },\n    \"employeeId\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The employee identifier assigned by the organization\"\n    },\n    \"employeeType\": {\n      \"type\": \"['string',\
  \ 'null']\",\n      \"description\": \"Captures the type of worker (e.g., Employee, Contractor, Consultant, Vendor)\"\n    },\n    \"employeeHireDate\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The date and time when the user was hired\"\n    },\n    \"onPremisesSyncEnabled\": {\n      \"type\": \"['boolean', 'null']\",\n      \"description\": \"true if this user is synced from an on-premises directory; false if originally created in Azure AD; null if never synced\"\n    },\n    \"onPremisesSamAccountName\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The on-premises SAM account name synchronized from the on-premises directory\"\n    },\n    \"proxyAddresses\": {\n      \"type\": \"array\",\n      \"description\": \"List of proxy addresses for the user including SMTP and smtp prefixed addresses\"\n    },\n    \"assignedLicenses\": {\n      \"type\": \"array\",\n      \"description\": \"Licenses assigned to the user\"\n    },\n    \"\
  createdDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the user was created\"\n    },\n    \"lastSignInDateTime\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The date and time of the user's most recent interactive sign-in activity\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra/refs/heads/main/json-schema/microsoft-entra-graph-identity-user-schema.json
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
title: User
---
