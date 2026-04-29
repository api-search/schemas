---
description: Schema for a Microsoft Entra ID (formerly Azure AD) user resource as represented in the Microsoft Graph API. Contains identity, contact, organizational, and authentication profile properties.
layout: schema
name: Microsoft Entra User
properties_list:
- description: Unique identifier for the user (GUID). Assigned automatically by Microsoft Entra ID.
  name: id
  type: string
- description: The name displayed in the address book for the user. Maximum length is 256 characters.
  name: displayName
  type: string
- description: The given name (first name) of the user. Maximum length is 64 characters.
  name: givenName
  type:
  - string
  - 'null'
- description: The surname (family name or last name) of the user. Maximum length is 64 characters.
  name: surname
  type:
  - string
  - 'null'
- description: The user principal name (UPN) in the format alias@domain. The domain portion must be a verified domain in the tenant.
  name: userPrincipalName
  type: string
- description: The SMTP address of the user (e.g., jeff@contoso.com). Changes to this property also update the proxyAddresses collection.
  name: mail
  type:
  - string
  - 'null'
- description: The mail alias for the user. Must be specified when creating a new user. Maximum length is 64 characters.
  name: mailNickname
  type: string
- description: true if the account is enabled; otherwise, false. Must be specified when creating a new user.
  name: accountEnabled
  type: boolean
- description: ''
  name: passwordProfile
  type: object
- description: The user's job title. Maximum length is 128 characters.
  name: jobTitle
  type:
  - string
  - 'null'
- description: The name of the department in which the user works. Maximum length is 64 characters.
  name: department
  type:
  - string
  - 'null'
- description: The office location in the user's place of business.
  name: officeLocation
  type:
  - string
  - 'null'
- description: The company name associated with the user. Maximum length is 64 characters.
  name: companyName
  type:
  - string
  - 'null'
- description: The primary cellular telephone number for the user. Maximum length is 64 characters.
  name: mobilePhone
  type:
  - string
  - 'null'
- description: The telephone numbers for the user. Only one number can be set. Read-only for users synced from on-premises.
  name: businessPhones
  type: array
- description: The street address of the user's place of business. Maximum length is 1024 characters.
  name: streetAddress
  type:
  - string
  - 'null'
- description: The city in which the user is located. Maximum length is 128 characters.
  name: city
  type:
  - string
  - 'null'
- description: The state or province in the user's address. Maximum length is 128 characters.
  name: state
  type:
  - string
  - 'null'
- description: The postal code for the user's postal address. Maximum length is 40 characters.
  name: postalCode
  type:
  - string
  - 'null'
- description: The country or region in which the user is located. Use ISO 3166 two-letter country code (e.g., US, GB).
  name: country
  type:
  - string
  - 'null'
- description: A two-letter country code (ISO 3166). Required for users assigned licenses due to legal requirements.
  name: usageLocation
  type:
  - string
  - 'null'
- description: The preferred language for the user in ISO 639-1 code format (e.g., en-US).
  name: preferredLanguage
  type:
  - string
  - 'null'
- description: A string value that classifies the user type. Member users are internal to the tenant, Guest users are invited from outside.
  name: userType
  type: string
- description: The employee identifier assigned to the user by the organization. Maximum length is 16 characters.
  name: employeeId
  type:
  - string
  - 'null'
- description: Captures the enterprise worker type (e.g., Employee, Contractor, Consultant, Vendor).
  name: employeeType
  type:
  - string
  - 'null'
- description: The date and time when the user was hired or will start work in a future hire.
  name: employeeHireDate
  type:
  - string
  - 'null'
- description: true if synced from an on-premises directory; false if originally cloud-created; null if never synced.
  name: onPremisesSyncEnabled
  type:
  - boolean
  - 'null'
- description: The on-premises SAM account name synchronized from the on-premises directory.
  name: onPremisesSamAccountName
  type:
  - string
  - 'null'
- description: The on-premises distinguished name (DN) synchronized from Active Directory.
  name: onPremisesDistinguishedName
  type:
  - string
  - 'null'
- description: The on-premises domain name synchronized from Active Directory.
  name: onPremisesDomainName
  type:
  - string
  - 'null'
- description: Used to associate an on-premises Active Directory user account to their Entra user object. Must be specified if using a federated domain for the UPN.
  name: onPremisesImmutableId
  type:
  - string
  - 'null'
- description: The last time the object was synced with the on-premises directory.
  name: onPremisesLastSyncDateTime
  type:
  - string
  - 'null'
- description: List of proxy addresses (e.g., SMTP:jeff@contoso.com, smtp:jeff@contoso.onmicrosoft.com).
  name: proxyAddresses
  type: array
- description: The licenses assigned to the user including disabled service plans.
  name: assignedLicenses
  type: array
- description: The plans assigned to the user.
  name: assignedPlans
  type: array
- description: Identities associated with the user account including social identities for B2B/B2C scenarios.
  name: identities
  type: array
- description: The date and time the user was created.
  name: createdDateTime
  type: string
- description: The last interactive sign-in date and time for the user.
  name: lastSignInDateTime
  type:
  - string
  - 'null'
- description: The date and time the user was deleted. Only present for deleted users in the deletedItems container.
  name: deletedDateTime
  type:
  - string
  - 'null'
provider_name: Microsoft Entra
provider_slug: microsoft-entra
schema_file: json-schema/microsoft-entra-user-schema.json
slug: microsoft-entra-user
source_filename: microsoft-entra-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://graph.microsoft.com/schemas/microsoft-entra/user.json\",\n  \"title\": \"Microsoft Entra User\",\n  \"description\": \"Schema for a Microsoft Entra ID (formerly Azure AD) user resource as represented in the Microsoft Graph API. Contains identity, contact, organizational, and authentication profile properties.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"displayName\",\n    \"accountEnabled\",\n    \"mailNickname\",\n    \"userPrincipalName\",\n    \"passwordProfile\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the user (GUID). Assigned automatically by Microsoft Entra ID.\",\n      \"readOnly\": true\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The name displayed in the address book for the user. Maximum length is 256 characters.\",\n      \"maxLength\": 256\n \
  \   },\n    \"givenName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The given name (first name) of the user. Maximum length is 64 characters.\",\n      \"maxLength\": 64\n    },\n    \"surname\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The surname (family name or last name) of the user. Maximum length is 64 characters.\",\n      \"maxLength\": 64\n    },\n    \"userPrincipalName\": {\n      \"type\": \"string\",\n      \"description\": \"The user principal name (UPN) in the format alias@domain. The domain portion must be a verified domain in the tenant.\",\n      \"format\": \"email\"\n    },\n    \"mail\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The SMTP address of the user (e.g., jeff@contoso.com). Changes to this property also update the proxyAddresses collection.\",\n      \"format\": \"email\"\n    },\n    \"mailNickname\": {\n      \"type\": \"string\",\n      \"description\": \"The mail alias for\
  \ the user. Must be specified when creating a new user. Maximum length is 64 characters.\",\n      \"maxLength\": 64\n    },\n    \"accountEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"true if the account is enabled; otherwise, false. Must be specified when creating a new user.\"\n    },\n    \"passwordProfile\": {\n      \"$ref\": \"#/$defs/PasswordProfile\"\n    },\n    \"jobTitle\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The user's job title. Maximum length is 128 characters.\",\n      \"maxLength\": 128\n    },\n    \"department\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The name of the department in which the user works. Maximum length is 64 characters.\",\n      \"maxLength\": 64\n    },\n    \"officeLocation\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The office location in the user's place of business.\",\n      \"maxLength\": 128\n    },\n    \"companyName\": {\n     \
  \ \"type\": [\"string\", \"null\"],\n      \"description\": \"The company name associated with the user. Maximum length is 64 characters.\",\n      \"maxLength\": 64\n    },\n    \"mobilePhone\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The primary cellular telephone number for the user. Maximum length is 64 characters.\",\n      \"maxLength\": 64\n    },\n    \"businessPhones\": {\n      \"type\": \"array\",\n      \"description\": \"The telephone numbers for the user. Only one number can be set. Read-only for users synced from on-premises.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"streetAddress\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The street address of the user's place of business. Maximum length is 1024 characters.\",\n      \"maxLength\": 1024\n    },\n    \"city\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The city in which the user is located. Maximum length\
  \ is 128 characters.\",\n      \"maxLength\": 128\n    },\n    \"state\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The state or province in the user's address. Maximum length is 128 characters.\",\n      \"maxLength\": 128\n    },\n    \"postalCode\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The postal code for the user's postal address. Maximum length is 40 characters.\",\n      \"maxLength\": 40\n    },\n    \"country\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The country or region in which the user is located. Use ISO 3166 two-letter country code (e.g., US, GB).\",\n      \"maxLength\": 128\n    },\n    \"usageLocation\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A two-letter country code (ISO 3166). Required for users assigned licenses due to legal requirements.\",\n      \"pattern\": \"^[A-Z]{2}$\"\n    },\n    \"preferredLanguage\": {\n      \"type\": [\"string\", \"null\"\
  ],\n      \"description\": \"The preferred language for the user in ISO 639-1 code format (e.g., en-US).\"\n    },\n    \"userType\": {\n      \"type\": \"string\",\n      \"description\": \"A string value that classifies the user type. Member users are internal to the tenant, Guest users are invited from outside.\",\n      \"enum\": [\"Member\", \"Guest\"]\n    },\n    \"employeeId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The employee identifier assigned to the user by the organization. Maximum length is 16 characters.\",\n      \"maxLength\": 16\n    },\n    \"employeeType\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Captures the enterprise worker type (e.g., Employee, Contractor, Consultant, Vendor).\"\n    },\n    \"employeeHireDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the user was hired or will start work in a future hire.\"\n    },\n\
  \    \"onPremisesSyncEnabled\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"true if synced from an on-premises directory; false if originally cloud-created; null if never synced.\",\n      \"readOnly\": true\n    },\n    \"onPremisesSamAccountName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The on-premises SAM account name synchronized from the on-premises directory.\",\n      \"readOnly\": true\n    },\n    \"onPremisesDistinguishedName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The on-premises distinguished name (DN) synchronized from Active Directory.\",\n      \"readOnly\": true\n    },\n    \"onPremisesDomainName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The on-premises domain name synchronized from Active Directory.\",\n      \"readOnly\": true\n    },\n    \"onPremisesImmutableId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Used to associate\
  \ an on-premises Active Directory user account to their Entra user object. Must be specified if using a federated domain for the UPN.\"\n    },\n    \"onPremisesLastSyncDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The last time the object was synced with the on-premises directory.\",\n      \"readOnly\": true\n    },\n    \"proxyAddresses\": {\n      \"type\": \"array\",\n      \"description\": \"List of proxy addresses (e.g., SMTP:jeff@contoso.com, smtp:jeff@contoso.onmicrosoft.com).\",\n      \"readOnly\": true,\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"assignedLicenses\": {\n      \"type\": \"array\",\n      \"description\": \"The licenses assigned to the user including disabled service plans.\",\n      \"readOnly\": true,\n      \"items\": {\n        \"$ref\": \"#/$defs/AssignedLicense\"\n      }\n    },\n    \"assignedPlans\": {\n      \"type\": \"array\",\n      \"description\":\
  \ \"The plans assigned to the user.\",\n      \"readOnly\": true,\n      \"items\": {\n        \"$ref\": \"#/$defs/AssignedPlan\"\n      }\n    },\n    \"identities\": {\n      \"type\": \"array\",\n      \"description\": \"Identities associated with the user account including social identities for B2B/B2C scenarios.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ObjectIdentity\"\n      }\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the user was created.\",\n      \"readOnly\": true\n    },\n    \"lastSignInDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The last interactive sign-in date and time for the user.\",\n      \"readOnly\": true\n    },\n    \"deletedDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the user was deleted. Only present\
  \ for deleted users in the deletedItems container.\",\n      \"readOnly\": true\n    }\n  },\n  \"$defs\": {\n    \"PasswordProfile\": {\n      \"type\": \"object\",\n      \"description\": \"Contains the password profile associated with a user including the password and policies for change enforcement.\",\n      \"required\": [\"password\"],\n      \"properties\": {\n        \"password\": {\n          \"type\": \"string\",\n          \"description\": \"The password for the user. Must satisfy the tenant's password complexity requirements. Required when creating a user.\",\n          \"writeOnly\": true\n        },\n        \"forceChangePasswordNextSignIn\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, the user must change the password on the next sign-in.\",\n          \"default\": false\n        },\n        \"forceChangePasswordNextSignInWithMfa\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, the user must perform MFA before\
  \ being forced to change password.\",\n          \"default\": false\n        }\n      }\n    },\n    \"AssignedLicense\": {\n      \"type\": \"object\",\n      \"description\": \"Represents a license assigned to a user.\",\n      \"properties\": {\n        \"disabledPlans\": {\n          \"type\": \"array\",\n          \"description\": \"Collection of the unique identifiers for plans that have been disabled.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          }\n        },\n        \"skuId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier for the SKU.\"\n        }\n      }\n    },\n    \"AssignedPlan\": {\n      \"type\": \"object\",\n      \"description\": \"Represents a plan assigned to a user.\",\n      \"properties\": {\n        \"assignedDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Date\
  \ and time the plan was assigned.\"\n        },\n        \"capabilityStatus\": {\n          \"type\": \"string\",\n          \"description\": \"Condition of the capability assignment.\",\n          \"enum\": [\"Enabled\", \"Warning\", \"Suspended\", \"Deleted\", \"LockedOut\"]\n        },\n        \"service\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the service (e.g., exchange, SharePoint).\"\n        },\n        \"servicePlanId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"GUID that identifies the service plan.\"\n        }\n      }\n    },\n    \"ObjectIdentity\": {\n      \"type\": \"object\",\n      \"description\": \"Represents an identity used to sign in to a user account, including social identities.\",\n      \"properties\": {\n        \"signInType\": {\n          \"type\": \"string\",\n          \"description\": \"Specifies the user sign-in type (e.g., emailAddress, userName, federated).\"\
  \n        },\n        \"issuer\": {\n          \"type\": \"string\",\n          \"description\": \"The issuer of the identity (e.g., contoso.com, facebook.com).\"\n        },\n        \"issuerAssignedId\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier assigned to the user by the issuer.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra/refs/heads/main/json-schema/microsoft-entra-user-schema.json
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
title: Microsoft Entra User
---
