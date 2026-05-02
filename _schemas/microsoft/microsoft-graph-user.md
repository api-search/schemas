---
description: Represents a Microsoft Entra user account. Inherits from directoryObject. Contains properties for identity, contact information, organizational role, and account settings managed through Microsoft Graph API.
layout: schema
name: Microsoft Graph User
properties_list:
- description: Unique identifier for the user (GUID). Inherited from directoryObject.
  name: id
  type: string
- description: Name displayed in the address book, usually the combination of first name, middle initial, and last name
  name: displayName
  type: string
- description: The given name (first name) of the user
  name: givenName
  type:
  - string
  - 'null'
- description: The user's last name (family name)
  name: surname
  type:
  - string
  - 'null'
- description: The SMTP address for the user
  name: mail
  type:
  - string
  - 'null'
- description: The user principal name (UPN) in internet-style login format based on RFC 822
  name: userPrincipalName
  type: string
- description: The mail alias for the user
  name: mailNickname
  type:
  - string
  - 'null'
- description: The user's job title
  name: jobTitle
  type:
  - string
  - 'null'
- description: The name of the department in which the user works
  name: department
  type:
  - string
  - 'null'
- description: The office location in the user's place of business
  name: officeLocation
  type:
  - string
  - 'null'
- description: The company name associated with the user
  name: companyName
  type:
  - string
  - 'null'
- description: Telephone numbers for the user
  name: businessPhones
  type: array
- description: The primary cellular telephone number for the user
  name: mobilePhone
  type:
  - string
  - 'null'
- description: The fax number of the user
  name: faxNumber
  type:
  - string
  - 'null'
- description: The street address of the user's place of business
  name: streetAddress
  type:
  - string
  - 'null'
- description: The city where the user is located
  name: city
  type:
  - string
  - 'null'
- description: The state or province in the user's address
  name: state
  type:
  - string
  - 'null'
- description: The postal code for the user's postal address
  name: postalCode
  type:
  - string
  - 'null'
- description: The country or region where the user is located
  name: country
  type:
  - string
  - 'null'
- description: A two-letter country code (ISO 3166) required for users assigned licenses
  name: usageLocation
  type:
  - string
  - 'null'
- description: The preferred language for the user in ISO 639-1 format (e.g., en-US)
  name: preferredLanguage
  type:
  - string
  - 'null'
- description: True if the account is enabled; otherwise, false
  name: accountEnabled
  type:
  - boolean
  - 'null'
- description: The employee identifier assigned to the user by the organization
  name: employeeId
  type:
  - string
  - 'null'
- description: Captures enterprise worker type (e.g., Employee, Contractor, Consultant, Vendor)
  name: employeeType
  type:
  - string
  - 'null'
- description: The date and time when the user was hired or will start work
  name: employeeHireDate
  type:
  - string
  - 'null'
- description: ''
  name: employeeOrgData
  type: object
- description: Sets the age group of the user
  name: ageGroup
  type:
  - string
  - 'null'
- description: Whether consent was obtained for minors
  name: consentProvidedForMinor
  type:
  - string
  - 'null'
- description: Legal age group classification used by enterprise applications
  name: legalAgeGroupClassification
  type:
  - string
  - 'null'
- description: The date and time the user was created in ISO 8601 format and UTC
  name: createdDateTime
  type:
  - string
  - 'null'
- description: The date and time the user was deleted
  name: deletedDateTime
  type:
  - string
  - 'null'
- description: The time when the user last changed their password
  name: lastPasswordChangeDateTime
  type:
  - string
  - 'null'
- description: Represents the identities that can be used to sign in to this user account
  name: identities
  type: array
- description: The instant message VoIP SIP addresses for the user
  name: imAddresses
  type: array
- description: Email addresses that direct to the same mailbox
  name: proxyAddresses
  type: array
- description: The licenses assigned to the user, including inherited group-based licenses
  name: assignedLicenses
  type: array
- description: The plans assigned to the user
  name: assignedPlans
  type: array
- description: True if the object is synced from an on-premises directory
  name: onPremisesSyncEnabled
  type:
  - boolean
  - 'null'
- description: Contains the on-premises Active Directory distinguished name
  name: onPremisesDistinguishedName
  type:
  - string
  - 'null'
- description: Contains the on-premises domain FQDN
  name: onPremisesDomainName
  type:
  - string
  - 'null'
- description: Last time the object was synced with the on-premises directory
  name: onPremisesLastSyncDateTime
  type:
  - string
  - 'null'
- description: Contains the on-premises SAM account name
  name: onPremisesSamAccountName
  type:
  - string
  - 'null'
- description: Contains the on-premises security identifier (SID)
  name: onPremisesSecurityIdentifier
  type:
  - string
  - 'null'
- description: Specifies password policies for the user
  name: passwordPolicies
  type:
  - string
  - 'null'
- description: ''
  name: passwordProfile
  type: object
- description: The URL for the user's personal site
  name: mySite
  type:
  - string
  - 'null'
- description: A freeform text entry field for the user to describe themselves
  name: aboutMe
  type:
  - string
  - 'null'
- description: A list for the user to describe their interests
  name: interests
  type: array
- description: The birthday of the user in ISO 8601 format and UTC
  name: birthday
  type:
  - string
  - 'null'
- description: For a guest invited to the tenant, this represents the invitation status
  name: externalUserState
  type:
  - string
  - 'null'
- description: Indicates how the user account was created
  name: creationType
  type:
  - string
  - 'null'
- description: Reserved for future use
  name: isResourceAccount
  type:
  - boolean
  - 'null'
provider_name: Microsoft
provider_slug: microsoft
schema_file: json-schema/microsoft-graph-user-schema.json
slug: microsoft-graph-user
source_filename: microsoft-graph-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://learn.microsoft.com/en-us/graph/schemas/microsoft/user.json\",\n  \"title\": \"Microsoft Graph User\",\n  \"description\": \"Represents a Microsoft Entra user account. Inherits from directoryObject. Contains properties for identity, contact information, organizational role, and account settings managed through Microsoft Graph API.\",\n  \"type\": \"object\",\n  \"required\": [\"displayName\", \"userPrincipalName\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the user (GUID). Inherited from directoryObject.\",\n      \"readOnly\": true\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Name displayed in the address book, usually the combination of first name, middle initial, and last name\",\n      \"maxLength\": 256\n    },\n    \"givenName\": {\n      \"type\": [\"string\", \"null\"\
  ],\n      \"description\": \"The given name (first name) of the user\",\n      \"maxLength\": 64\n    },\n    \"surname\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The user's last name (family name)\",\n      \"maxLength\": 64\n    },\n    \"mail\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"email\",\n      \"description\": \"The SMTP address for the user\"\n    },\n    \"userPrincipalName\": {\n      \"type\": \"string\",\n      \"description\": \"The user principal name (UPN) in internet-style login format based on RFC 822\"\n    },\n    \"mailNickname\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The mail alias for the user\",\n      \"maxLength\": 64\n    },\n    \"jobTitle\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The user's job title\",\n      \"maxLength\": 128\n    },\n    \"department\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The name of the department\
  \ in which the user works\",\n      \"maxLength\": 64\n    },\n    \"officeLocation\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The office location in the user's place of business\"\n    },\n    \"companyName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The company name associated with the user\",\n      \"maxLength\": 64\n    },\n    \"businessPhones\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Telephone numbers for the user\"\n    },\n    \"mobilePhone\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The primary cellular telephone number for the user\",\n      \"maxLength\": 64\n    },\n    \"faxNumber\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The fax number of the user\"\n    },\n    \"streetAddress\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The street address of the user's place\
  \ of business\",\n      \"maxLength\": 1024\n    },\n    \"city\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The city where the user is located\",\n      \"maxLength\": 128\n    },\n    \"state\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The state or province in the user's address\",\n      \"maxLength\": 128\n    },\n    \"postalCode\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The postal code for the user's postal address\",\n      \"maxLength\": 40\n    },\n    \"country\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The country or region where the user is located\",\n      \"maxLength\": 128\n    },\n    \"usageLocation\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A two-letter country code (ISO 3166) required for users assigned licenses\",\n      \"minLength\": 2,\n      \"maxLength\": 2\n    },\n    \"preferredLanguage\": {\n      \"type\": [\"string\"\
  , \"null\"],\n      \"description\": \"The preferred language for the user in ISO 639-1 format (e.g., en-US)\"\n    },\n    \"accountEnabled\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"True if the account is enabled; otherwise, false\"\n    },\n    \"employeeId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The employee identifier assigned to the user by the organization\",\n      \"maxLength\": 16\n    },\n    \"employeeType\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Captures enterprise worker type (e.g., Employee, Contractor, Consultant, Vendor)\"\n    },\n    \"employeeHireDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the user was hired or will start work\"\n    },\n    \"employeeOrgData\": {\n      \"$ref\": \"#/$defs/EmployeeOrgData\"\n    },\n    \"ageGroup\": {\n      \"type\": [\"string\", \"null\"],\n      \"\
  enum\": [null, \"Minor\", \"NotAdult\", \"Adult\"],\n      \"description\": \"Sets the age group of the user\"\n    },\n    \"consentProvidedForMinor\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [null, \"Granted\", \"Denied\", \"NotRequired\"],\n      \"description\": \"Whether consent was obtained for minors\"\n    },\n    \"legalAgeGroupClassification\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [null, \"Undefined\", \"MinorWithOutParentalConsent\", \"MinorWithParentalConsent\", \"MinorNoParentalConsentRequired\", \"NotAdult\", \"Adult\"],\n      \"description\": \"Legal age group classification used by enterprise applications\",\n      \"readOnly\": true\n    },\n    \"createdDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the user was created in ISO 8601 format and UTC\",\n      \"readOnly\": true\n    },\n    \"deletedDateTime\": {\n      \"type\": [\"string\",\
  \ \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the user was deleted\",\n      \"readOnly\": true\n    },\n    \"lastPasswordChangeDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The time when the user last changed their password\",\n      \"readOnly\": true\n    },\n    \"identities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ObjectIdentity\"\n      },\n      \"description\": \"Represents the identities that can be used to sign in to this user account\"\n    },\n    \"imAddresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The instant message VoIP SIP addresses for the user\",\n      \"readOnly\": true\n    },\n    \"proxyAddresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Email addresses that\
  \ direct to the same mailbox\",\n      \"readOnly\": true\n    },\n    \"assignedLicenses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AssignedLicense\"\n      },\n      \"description\": \"The licenses assigned to the user, including inherited group-based licenses\"\n    },\n    \"assignedPlans\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AssignedPlan\"\n      },\n      \"description\": \"The plans assigned to the user\",\n      \"readOnly\": true\n    },\n    \"onPremisesSyncEnabled\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"True if the object is synced from an on-premises directory\",\n      \"readOnly\": true\n    },\n    \"onPremisesDistinguishedName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Contains the on-premises Active Directory distinguished name\",\n      \"readOnly\": true\n    },\n    \"onPremisesDomainName\": {\n      \"type\": [\"string\",\
  \ \"null\"],\n      \"description\": \"Contains the on-premises domain FQDN\",\n      \"readOnly\": true\n    },\n    \"onPremisesLastSyncDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Last time the object was synced with the on-premises directory\",\n      \"readOnly\": true\n    },\n    \"onPremisesSamAccountName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Contains the on-premises SAM account name\",\n      \"readOnly\": true\n    },\n    \"onPremisesSecurityIdentifier\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Contains the on-premises security identifier (SID)\",\n      \"readOnly\": true\n    },\n    \"passwordPolicies\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Specifies password policies for the user\"\n    },\n    \"passwordProfile\": {\n      \"$ref\": \"#/$defs/PasswordProfile\"\n    },\n    \"mySite\": {\n      \"type\": [\"\
  string\", \"null\"],\n      \"description\": \"The URL for the user's personal site\"\n    },\n    \"aboutMe\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A freeform text entry field for the user to describe themselves\"\n    },\n    \"interests\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A list for the user to describe their interests\"\n    },\n    \"birthday\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The birthday of the user in ISO 8601 format and UTC\"\n    },\n    \"externalUserState\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [null, \"PendingAcceptance\", \"Accepted\"],\n      \"description\": \"For a guest invited to the tenant, this represents the invitation status\"\n    },\n    \"creationType\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Indicates how the user account was\
  \ created\",\n      \"readOnly\": true\n    },\n    \"isResourceAccount\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Reserved for future use\"\n    }\n  },\n  \"$defs\": {\n    \"EmployeeOrgData\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Represents organization data associated with a user\",\n      \"properties\": {\n        \"division\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The name of the division in which the user works\"\n        },\n        \"costCenter\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The cost center associated with the user\"\n        }\n      }\n    },\n    \"ObjectIdentity\": {\n      \"type\": \"object\",\n      \"description\": \"Represents an identity used to sign in to a user account\",\n      \"properties\": {\n        \"signInType\": {\n          \"type\": \"string\",\n          \"description\": \"Specifies the user sign-in type\
  \ (e.g., emailAddress, userName, federated)\"\n        },\n        \"issuer\": {\n          \"type\": \"string\",\n          \"description\": \"Specifies the issuer of the identity\"\n        },\n        \"issuerAssignedId\": {\n          \"type\": \"string\",\n          \"description\": \"Specifies the unique identifier assigned to the user by the issuer\"\n        }\n      }\n    },\n    \"AssignedLicense\": {\n      \"type\": \"object\",\n      \"description\": \"Represents a license assigned to a user\",\n      \"properties\": {\n        \"skuId\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for the SKU\"\n        },\n        \"disabledPlans\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"A collection of the unique identifiers for disabled plans\"\n        }\n      }\n    },\n    \"AssignedPlan\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Represents a plan assigned to a user\",\n      \"properties\": {\n        \"assignedDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time at which the plan was assigned\"\n        },\n        \"capabilityStatus\": {\n          \"type\": \"string\",\n          \"enum\": [\"Enabled\", \"Warning\", \"Suspended\", \"Deleted\", \"LockedOut\"],\n          \"description\": \"Condition of the capability assignment\"\n        },\n        \"service\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the service\"\n        },\n        \"servicePlanId\": {\n          \"type\": \"string\",\n          \"description\": \"A GUID that identifies the service plan\"\n        }\n      }\n    },\n    \"PasswordProfile\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Contains the password profile associated with a user\",\n      \"properties\": {\n        \"forceChangePasswordNextSignIn\"\
  : {\n          \"type\": \"boolean\",\n          \"description\": \"If true, at next sign-in the user must change their password\"\n        },\n        \"forceChangePasswordNextSignInWithMfa\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, at next sign-in the user must perform MFA before changing their password\"\n        },\n        \"password\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The password for the user. Required when creating a user.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/json-schema/microsoft-graph-user-schema.json
tags: []
title: Microsoft Graph User
---
