---
description: Represents a Microsoft Entra ID user account. Users are the core identity objects in Microsoft Graph and serve as the principal entity for accessing Microsoft 365 services including Outlook mail, calendar, OneDrive files, Teams, and more. Each user has a unique identifier, profile information, authentication credentials, and relationships to groups, roles, and organizational resources.
layout: schema
name: Microsoft Graph User
properties_list:
- description: The unique identifier for the user. Assigned by Microsoft Entra ID upon creation. Read-only.
  name: id
  type: string
- description: The name displayed in the address book for the user. This value is usually the combination of the user's first name, middle initial, and last name.
  name: displayName
  type: string
- description: The given name (first name) of the user.
  name: givenName
  type:
  - string
  - 'null'
- description: The user's surname (family name or last name).
  name: surname
  type:
  - string
  - 'null'
- description: The SMTP address for the user. Read-only for cloud-only users; writable for on-premises synced users.
  name: mail
  type:
  - string
  - 'null'
- description: The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.
  name: userPrincipalName
  type: string
- description: The mail alias for the user. This property must be specified when a user is created.
  name: mailNickname
  type: string
- description: True if the account is enabled; otherwise, false. This property is required when a user is created.
  name: accountEnabled
  type: boolean
- description: The user's job title.
  name: jobTitle
  type:
  - string
  - 'null'
- description: The name of the department in which the user works.
  name: department
  type:
  - string
  - 'null'
- description: The office location in the user's place of business.
  name: officeLocation
  type:
  - string
  - 'null'
- description: The company name associated with the user.
  name: companyName
  type:
  - string
  - 'null'
- description: The primary cellular telephone number for the user.
  name: mobilePhone
  type:
  - string
  - 'null'
- description: The telephone numbers for the user. Only one number can be set for this property.
  name: businessPhones
  type: array
- description: The street address of the user's place of business.
  name: streetAddress
  type:
  - string
  - 'null'
- description: The city in which the user is located.
  name: city
  type:
  - string
  - 'null'
- description: The state or province in the user's address.
  name: state
  type:
  - string
  - 'null'
- description: The postal code for the user's postal address.
  name: postalCode
  type:
  - string
  - 'null'
- description: The country or region in which the user is located; for example, US or UK.
  name: country
  type:
  - string
  - 'null'
- description: A two-letter country code (ISO standard 3166) required for users assigned licenses due to legal requirements for checking availability of services in countries.
  name: usageLocation
  type:
  - string
  - 'null'
- description: The preferred language for the user, in ISO 639-1 code format.
  name: preferredLanguage
  type:
  - string
  - 'null'
- description: A string value that can be used to classify user types in your directory, such as Member and Guest.
  name: userType
  type:
  - string
  - 'null'
- description: The employee identifier assigned to the user by the organization.
  name: employeeId
  type:
  - string
  - 'null'
- description: Captures enterprise worker type, such as Employee, Contractor, Consultant, or Vendor.
  name: employeeType
  type:
  - string
  - 'null'
- description: The date and time when the user was hired or will start work in case of a future hire.
  name: employeeHireDate
  type:
  - string
  - 'null'
- description: The date and time the user was created. Read-only.
  name: createdDateTime
  type: string
- description: The time when this user last changed their password. Read-only.
  name: lastPasswordChangeDateTime
  type:
  - string
  - 'null'
- description: ''
  name: signInActivity
  type: object
- description: The licenses that are assigned to the user, including inherited group-based licenses.
  name: assignedLicenses
  type: array
- description: The plans that are assigned to the user.
  name: assignedPlans
  type: array
- description: The plans that are provisioned for the user. Read-only.
  name: provisionedPlans
  type: array
- description: Represents the identities that can be used to sign in to this user account, including the standard identity (sign-in with UPN) and social or local account identities.
  name: identities
  type: array
- description: True if this user object is currently being synced from an on-premises Active Directory; otherwise false or null. Read-only.
  name: onPremisesSyncEnabled
  type:
  - boolean
  - 'null'
- description: This property is used to associate an on-premises Active Directory user account to their Azure AD user object.
  name: onPremisesImmutableId
  type:
  - string
  - 'null'
- description: The last time at which the object was synced with the on-premises directory. Read-only.
  name: onPremisesLastSyncDateTime
  type:
  - string
  - 'null'
- description: 'Email addresses associated with the user. For example: [''SMTP:bob@contoso.com'', ''smtp:bob@sales.contoso.com''].'
  name: proxyAddresses
  type: array
- description: The date and time the user was deleted. Read-only.
  name: deletedDateTime
  type:
  - string
  - 'null'
provider_name: Microsoft Graph
provider_slug: microsoft-graph
schema_file: json-schema/microsoft-graph-user-schema.json
slug: microsoft-graph-user
source_filename: microsoft-graph-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.api.gov/microsoft-graph/user\",\n  \"title\": \"Microsoft Graph User\",\n  \"description\": \"Represents a Microsoft Entra ID user account. Users are the core identity objects in Microsoft Graph and serve as the principal entity for accessing Microsoft 365 services including Outlook mail, calendar, OneDrive files, Teams, and more. Each user has a unique identifier, profile information, authentication credentials, and relationships to groups, roles, and organizational resources.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"displayName\",\n    \"mailNickname\",\n    \"userPrincipalName\",\n    \"accountEnabled\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the user. Assigned by Microsoft Entra ID upon creation. Read-only.\",\n      \"readOnly\": true,\n      \"examples\": [\n        \"87d349ed-44d7-43e1-9a83-5f2406dee5bd\"\
  \n      ]\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The name displayed in the address book for the user. This value is usually the combination of the user's first name, middle initial, and last name.\",\n      \"maxLength\": 256,\n      \"examples\": [\n        \"Adele Vance\"\n      ]\n    },\n    \"givenName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The given name (first name) of the user.\",\n      \"maxLength\": 64,\n      \"examples\": [\n        \"Adele\"\n      ]\n    },\n    \"surname\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The user's surname (family name or last name).\",\n      \"maxLength\": 64,\n      \"examples\": [\n        \"Vance\"\n      ]\n    },\n    \"mail\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The SMTP address for the user. Read-only for cloud-only users; writable for on-premises synced users.\",\n      \"format\": \"email\",\n\
  \      \"examples\": [\n        \"adelev@contoso.com\"\n      ]\n    },\n    \"userPrincipalName\": {\n      \"type\": \"string\",\n      \"description\": \"The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.\",\n      \"examples\": [\n        \"adelev@contoso.com\"\n      ]\n    },\n    \"mailNickname\": {\n      \"type\": \"string\",\n      \"description\": \"The mail alias for the user. This property must be specified when a user is created.\",\n      \"maxLength\": 64,\n      \"examples\": [\n        \"adelev\"\n      ]\n    },\n    \"accountEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the account is enabled; otherwise, false. This property is required when a user is created.\"\n    },\n    \"jobTitle\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The user's job title.\",\n      \"maxLength\": 128,\n      \"examples\": [\n        \"Retail Manager\"\
  \n      ]\n    },\n    \"department\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The name of the department in which the user works.\",\n      \"maxLength\": 64,\n      \"examples\": [\n        \"Retail\"\n      ]\n    },\n    \"officeLocation\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The office location in the user's place of business.\",\n      \"maxLength\": 128\n    },\n    \"companyName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The company name associated with the user.\",\n      \"maxLength\": 64\n    },\n    \"mobilePhone\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The primary cellular telephone number for the user.\",\n      \"examples\": [\n        \"+1 425 555 0109\"\n      ]\n    },\n    \"businessPhones\": {\n      \"type\": \"array\",\n      \"description\": \"The telephone numbers for the user. Only one number can be set for this property.\",\n      \"items\"\
  : {\n        \"type\": \"string\"\n      }\n    },\n    \"streetAddress\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The street address of the user's place of business.\",\n      \"maxLength\": 1024\n    },\n    \"city\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The city in which the user is located.\",\n      \"maxLength\": 128\n    },\n    \"state\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The state or province in the user's address.\",\n      \"maxLength\": 128\n    },\n    \"postalCode\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The postal code for the user's postal address.\",\n      \"maxLength\": 40\n    },\n    \"country\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The country or region in which the user is located; for example, US or UK.\",\n      \"maxLength\": 128\n    },\n    \"usageLocation\": {\n      \"type\": [\"string\", \"null\"],\n\
  \      \"description\": \"A two-letter country code (ISO standard 3166) required for users assigned licenses due to legal requirements for checking availability of services in countries.\",\n      \"pattern\": \"^[A-Z]{2}$\",\n      \"examples\": [\n        \"US\"\n      ]\n    },\n    \"preferredLanguage\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The preferred language for the user, in ISO 639-1 code format.\",\n      \"examples\": [\n        \"en-US\"\n      ]\n    },\n    \"userType\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A string value that can be used to classify user types in your directory, such as Member and Guest.\",\n      \"enum\": [\"Member\", \"Guest\", null]\n    },\n    \"employeeId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The employee identifier assigned to the user by the organization.\",\n      \"maxLength\": 16\n    },\n    \"employeeType\": {\n      \"type\": [\"string\", \"\
  null\"],\n      \"description\": \"Captures enterprise worker type, such as Employee, Contractor, Consultant, or Vendor.\"\n    },\n    \"employeeHireDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the user was hired or will start work in case of a future hire.\"\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the user was created. Read-only.\",\n      \"readOnly\": true\n    },\n    \"lastPasswordChangeDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The time when this user last changed their password. Read-only.\",\n      \"readOnly\": true\n    },\n    \"signInActivity\": {\n      \"$ref\": \"#/$defs/SignInActivity\"\n    },\n    \"assignedLicenses\": {\n      \"type\": \"array\",\n      \"description\": \"The licenses that are assigned to\
  \ the user, including inherited group-based licenses.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AssignedLicense\"\n      }\n    },\n    \"assignedPlans\": {\n      \"type\": \"array\",\n      \"description\": \"The plans that are assigned to the user.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AssignedPlan\"\n      }\n    },\n    \"provisionedPlans\": {\n      \"type\": \"array\",\n      \"description\": \"The plans that are provisioned for the user. Read-only.\",\n      \"readOnly\": true,\n      \"items\": {\n        \"$ref\": \"#/$defs/ProvisionedPlan\"\n      }\n    },\n    \"identities\": {\n      \"type\": \"array\",\n      \"description\": \"Represents the identities that can be used to sign in to this user account, including the standard identity (sign-in with UPN) and social or local account identities.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ObjectIdentity\"\n      }\n    },\n    \"onPremisesSyncEnabled\": {\n      \"type\": [\"boolean\", \"null\"\
  ],\n      \"description\": \"True if this user object is currently being synced from an on-premises Active Directory; otherwise false or null. Read-only.\",\n      \"readOnly\": true\n    },\n    \"onPremisesImmutableId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"This property is used to associate an on-premises Active Directory user account to their Azure AD user object.\"\n    },\n    \"onPremisesLastSyncDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The last time at which the object was synced with the on-premises directory. Read-only.\",\n      \"readOnly\": true\n    },\n    \"proxyAddresses\": {\n      \"type\": \"array\",\n      \"description\": \"Email addresses associated with the user. For example: ['SMTP:bob@contoso.com', 'smtp:bob@sales.contoso.com'].\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"deletedDateTime\": {\n      \"type\": [\"string\", \"\
  null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the user was deleted. Read-only.\",\n      \"readOnly\": true\n    }\n  },\n  \"$defs\": {\n    \"SignInActivity\": {\n      \"type\": \"object\",\n      \"description\": \"Provides the last interactive and non-interactive sign-in date and time and the corresponding request ID for the user.\",\n      \"properties\": {\n        \"lastSignInDateTime\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date-time\",\n          \"description\": \"The last interactive sign-in date and time for a specific user.\"\n        },\n        \"lastSignInRequestId\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Request identifier of the last interactive sign-in performed by this user.\"\n        },\n        \"lastNonInteractiveSignInDateTime\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date-time\",\n          \"description\": \"The last\
  \ non-interactive sign-in date for a specific user.\"\n        },\n        \"lastNonInteractiveSignInRequestId\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Request identifier of the last non-interactive sign-in performed by this user.\"\n        }\n      }\n    },\n    \"AssignedLicense\": {\n      \"type\": \"object\",\n      \"description\": \"Represents a license assigned to a user, identifying the SKU and any disabled service plans.\",\n      \"properties\": {\n        \"disabledPlans\": {\n          \"type\": \"array\",\n          \"description\": \"A collection of the unique identifiers for plans that have been disabled.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          }\n        },\n        \"skuId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier for the SKU.\"\n        }\n      }\n    },\n    \"AssignedPlan\": {\n\
  \      \"type\": \"object\",\n      \"description\": \"Represents a plan assigned to a user.\",\n      \"properties\": {\n        \"assignedDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time at which the plan was assigned.\"\n        },\n        \"capabilityStatus\": {\n          \"type\": \"string\",\n          \"description\": \"Condition of the capability assignment, such as Enabled, Warning, Suspended, Deleted, LockedOut.\",\n          \"enum\": [\n            \"Enabled\",\n            \"Warning\",\n            \"Suspended\",\n            \"Deleted\",\n            \"LockedOut\"\n          ]\n        },\n        \"service\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the service; for example, exchange.\"\n        },\n        \"servicePlanId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"A GUID that identifies the service\
  \ plan.\"\n        }\n      }\n    },\n    \"ProvisionedPlan\": {\n      \"type\": \"object\",\n      \"description\": \"Represents a service plan that has been provisioned for the user.\",\n      \"properties\": {\n        \"capabilityStatus\": {\n          \"type\": \"string\",\n          \"description\": \"The provisioning status, such as Enabled.\"\n        },\n        \"provisioningStatus\": {\n          \"type\": \"string\",\n          \"description\": \"The provisioning status, such as Success.\"\n        },\n        \"service\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the service; for example, SharePoint, Exchange.\"\n        }\n      }\n    },\n    \"ObjectIdentity\": {\n      \"type\": \"object\",\n      \"description\": \"Represents an identity used to sign in to a user account.\",\n      \"properties\": {\n        \"signInType\": {\n          \"type\": \"string\",\n          \"description\": \"Specifies the user sign-in type, such as emailAddress,\
  \ userName, or federated.\"\n        },\n        \"issuer\": {\n          \"type\": \"string\",\n          \"description\": \"Specifies the issuer of the identity, for example contoso.onmicrosoft.com.\"\n        },\n        \"issuerAssignedId\": {\n          \"type\": \"string\",\n          \"description\": \"Specifies the unique identifier assigned to the user by the issuer.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-graph/refs/heads/main/json-schema/microsoft-graph-user-schema.json
tags:
- Azure AD
- Collaboration
- Contacts
- Documents
- Email
- Graph
- Identity
- Microsoft
- Office 365
- Presentations
- Productivity
- Spreadsheets
- T1
- Tasks
title: Microsoft Graph User
---
