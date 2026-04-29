---
description: Represents a user account in Azure Active Directory (Microsoft Entra ID). A user is a core identity object in the Microsoft identity platform, containing profile information, authentication credentials, organizational relationships, and license assignments. This schema is based on the Microsoft Graph v1.0 user resource type as documented at https://learn.microsoft.com/en-us/graph/api/resources/user.
layout: schema
name: Azure Active Directory User
properties_list:
- description: The OData type annotation for the user resource.
  name: '@odata.type'
  type: string
- description: The unique identifier for the user. This is a GUID assigned by Azure AD when the user object is created. Read-only.
  name: id
  type: string
- description: The date and time the user was deleted. Null if the user has not been deleted. Read-only.
  name: deletedDateTime
  type:
  - string
  - 'null'
- description: True if the account is enabled; otherwise, false. This property is required when creating a user. A disabled account cannot authenticate.
  name: accountEnabled
  type: boolean
- description: 'Sets the age group of the user. Allowed values: null, Minor, NotAdult, Adult.'
  name: ageGroup
  type:
  - string
  - 'null'
- description: The licenses assigned to the user, including specific disabled service plans. Read-only. Not nullable.
  name: assignedLicenses
  type: array
- description: The plans assigned to the user from subscriptions. Read-only. Not nullable.
  name: assignedPlans
  type: array
- description: The telephone numbers for the user. Only one number can be set for this property. Read-only for users synced from on-premises directory.
  name: businessPhones
  type: array
- description: The city where the user is located. Maximum length is 128 characters.
  name: city
  type:
  - string
  - 'null'
- description: The name of the company associated with the user. This property can be useful for describing the company that an external user comes from. Maximum length is 64 characters.
  name: companyName
  type:
  - string
  - 'null'
- description: 'Sets whether consent was obtained for minors. Allowed values: null, Granted, Denied, NotRequired.'
  name: consentProvidedForMinor
  type:
  - string
  - 'null'
- description: The country or region where the user is located. Use the ISO 3166 two-letter country code format (e.g., US, GB, DE). Maximum length is 128 characters.
  name: country
  type:
  - string
  - 'null'
- description: The date and time the user was created in ISO 8601 format and UTC time. Read-only.
  name: createdDateTime
  type:
  - string
  - 'null'
- description: 'Indicates whether the user account was created through one of the following methods: as a regular school or work account (null), as an external account (Invitation), as a local account for an Azure Ac'
  name: creationType
  type:
  - string
  - 'null'
- description: The name of the department in which the user works. Maximum length is 64 characters.
  name: department
  type:
  - string
  - 'null'
- description: The name displayed in the address book for the user. This is usually the combination of the first name, middle initial, and last name. This property is required when a user is created and cannot be cl
  name: displayName
  type: string
- description: The date and time when the user was hired or will start work in case of a future hire.
  name: employeeHireDate
  type:
  - string
  - 'null'
- description: The employee identifier assigned to the user by the organization. The maximum length is 16 characters.
  name: employeeId
  type:
  - string
  - 'null'
- description: The date and time when the user left or will leave the organization.
  name: employeeLeaveDateTime
  type:
  - string
  - 'null'
- description: Represents organization data (e.g., division and costCenter) associated with a user.
  name: employeeOrgData
  type: object
- description: Captures enterprise worker type. For example, Employee, Contractor, Consultant, or Vendor.
  name: employeeType
  type:
  - string
  - 'null'
- description: 'For an external user invited to the tenant, this property represents the invited user''s invitation status. Possible values: PendingAcceptance, Accepted, null. Read-only.'
  name: externalUserState
  type:
  - string
  - 'null'
- description: Shows the timestamp for the latest change to the externalUserState property. Read-only.
  name: externalUserStateChangeDateTime
  type:
  - string
  - 'null'
- description: The fax number of the user.
  name: faxNumber
  type:
  - string
  - 'null'
- description: The given name (first name) of the user. Maximum length is 64 characters.
  name: givenName
  type:
  - string
  - 'null'
- description: Represents the identities that can be used to sign in to this user account. An identity can be provided by Microsoft, by organizations, or by social identity providers. May contain multiple items with
  name: identities
  type: array
- description: The instant message voice-over-IP (VOIP) session initiation protocol (SIP) addresses for the user. Read-only.
  name: imAddresses
  type: array
- description: Do not use. Reserved for future use.
  name: isResourceAccount
  type:
  - boolean
  - 'null'
- description: The user's job title. Maximum length is 128 characters.
  name: jobTitle
  type:
  - string
  - 'null'
- description: The time when this Azure AD user last changed their password or when their password was created. Read-only.
  name: lastPasswordChangeDateTime
  type:
  - string
  - 'null'
- description: Used by enterprise applications to determine the legal age group of the user. Read-only.
  name: legalAgeGroupClassification
  type:
  - string
  - 'null'
- description: State of license assignments for this user. Read-only.
  name: licenseAssignmentStates
  type: array
- description: The SMTP address for the user (e.g., admin@contoso.com). Changes to this property also update the user's proxyAddresses collection to include the value as an SMTP address. This property cannot contain
  name: mail
  type:
  - string
  - 'null'
- description: The mail alias for the user. This property must be specified when a user is created. Maximum length is 64 characters.
  name: mailNickname
  type: string
- description: The primary cellular telephone number for the user. Read-only for users synced from on-premises directory.
  name: mobilePhone
  type:
  - string
  - 'null'
- description: The office location in the user's place of business.
  name: officeLocation
  type:
  - string
  - 'null'
- description: Contains the on-premises Active Directory distinguished name or DN. Read-only.
  name: onPremisesDistinguishedName
  type:
  - string
  - 'null'
- description: Contains the on-premises domainFQDN, also called dnsDomainName, synced from the on-premises directory. Read-only.
  name: onPremisesDomainName
  type:
  - string
  - 'null'
- description: Contains extensionAttributes1-15 for the user. These extension attributes are also known as Exchange custom attributes. Read-only for cloud-only users.
  name: onPremisesExtensionAttributes
  type: object
- description: This property is used to associate an on-premises Active Directory user account to their Azure AD user object. This property must be specified when creating a new user if you are using a federated dom
  name: onPremisesImmutableId
  type:
  - string
  - 'null'
- description: Indicates the last time at which the object was synced with the on-premises directory. Read-only.
  name: onPremisesLastSyncDateTime
  type:
  - string
  - 'null'
- description: Errors when using Microsoft synchronization product during provisioning. Read-only.
  name: onPremisesProvisioningErrors
  type: array
- description: Contains the on-premises samAccountName synced from the on-premises directory. Read-only.
  name: onPremisesSamAccountName
  type:
  - string
  - 'null'
- description: Contains the on-premises security identifier (SID) for the user that was synced from on-premises to the cloud. Read-only.
  name: onPremisesSecurityIdentifier
  type:
  - string
  - 'null'
- description: True if this user object is currently being synced from an on-premises Active Directory (AD); otherwise, the user isn't being synced and can be managed in Azure Active Directory. Read-only.
  name: onPremisesSyncEnabled
  type:
  - boolean
  - 'null'
- description: Contains the on-premises userPrincipalName synced from the on-premises directory. Read-only.
  name: onPremisesUserPrincipalName
  type:
  - string
  - 'null'
- description: A list of additional email addresses for the user (e.g., ["bob@contoso.com", "Robert@fabrikam.com"]).
  name: otherMails
  type: array
- description: Specifies password policies for the user. This value is an enumeration with one possible value being DisableStrongPassword, which allows weaker passwords than the default policy to be specified. Disab
  name: passwordPolicies
  type:
  - string
  - 'null'
- description: Specifies the password profile for the user. The profile contains the user's password. This property is required when a user is created.
  name: passwordProfile
  type: object
- description: The postal code for the user's postal address. The postal code is specific to the user's country/region. Maximum length is 40 characters.
  name: postalCode
  type:
  - string
  - 'null'
- description: The preferred language for the user, expressed in ISO 639-1 code format (e.g., en-US).
  name: preferredLanguage
  type:
  - string
  - 'null'
- description: The preferred data location for the user, indicating the geographic region for their data.
  name: preferredDataLocation
  type:
  - string
  - 'null'
- description: The plans that are provisioned for the user. Read-only. Not nullable.
  name: provisionedPlans
  type: array
- description: 'A list that includes the user''s SMTP and SIP proxy addresses. For example: ["SMTP:bob@contoso.com", "smtp:bob@sales.contoso.com"]. The address prefixed with SMTP (uppercase) is the primary. Read-only.'
  name: proxyAddresses
  type: array
- description: Security identifier (SID) of the user, used in Windows scenarios. Read-only.
  name: securityIdentifier
  type:
  - string
  - 'null'
- description: Do not use in Microsoft Graph. Manage this property through the Microsoft 365 admin center instead.
  name: showInAddressList
  type:
  - boolean
  - 'null'
- description: Get the last signed-in date and request ID of the sign-in for a given user. Read-only. Requires Azure AD Premium P1 or P2 license.
  name: signInActivity
  type: object
- description: Any refresh tokens or sessions tokens (session cookies) issued before this time are invalid, and applications will get an error when using an invalid refresh or sessions token to acquire a delegated a
  name: signInSessionsValidFromDateTime
  type:
  - string
  - 'null'
- description: The state or province in the user's address. Maximum length is 128 characters.
  name: state
  type:
  - string
  - 'null'
- description: The street address of the user's place of business. Maximum length is 1024 characters.
  name: streetAddress
  type:
  - string
  - 'null'
- description: The user's surname (family name or last name). Maximum length is 64 characters.
  name: surname
  type:
  - string
  - 'null'
- description: 'A two-letter country code (ISO standard 3166). Required for users that will be assigned licenses due to legal requirements to check for availability of services in countries/regions. Examples include '
  name: usageLocation
  type:
  - string
  - 'null'
- description: The user principal name (UPN) of the user. The UPN is an Internet-style sign-in name based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format
  name: userPrincipalName
  type: string
- description: A string value that can be used to classify user types in your directory, such as Member and Guest.
  name: userType
  type:
  - string
  - 'null'
provider_name: Azure Active Directory
provider_slug: azure-active-directory
schema_file: json-schema/azure-active-directory-user-schema.json
slug: azure-active-directory-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.api.gov/azure-active-directory/user\",\n  \"title\": \"Azure Active Directory User\",\n  \"description\": \"Represents a user account in Azure Active Directory (Microsoft Entra ID). A user is a core identity object in the Microsoft identity platform, containing profile information, authentication credentials, organizational relationships, and license assignments. This schema is based on the Microsoft Graph v1.0 user resource type as documented at https://learn.microsoft.com/en-us/graph/api/resources/user.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"displayName\",\n    \"userPrincipalName\"\n  ],\n  \"properties\": {\n    \"@odata.type\": {\n      \"type\": \"string\",\n      \"const\": \"#microsoft.graph.user\",\n      \"description\": \"The OData type annotation for the user resource.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n\
  \      \"description\": \"The unique identifier for the user. This is a GUID assigned by Azure AD when the user object is created. Read-only.\",\n      \"readOnly\": true\n    },\n    \"deletedDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the user was deleted. Null if the user has not been deleted. Read-only.\",\n      \"readOnly\": true\n    },\n    \"accountEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the account is enabled; otherwise, false. This property is required when creating a user. A disabled account cannot authenticate.\"\n    },\n    \"ageGroup\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Sets the age group of the user. Allowed values: null, Minor, NotAdult, Adult.\",\n      \"enum\": [null, \"Minor\", \"NotAdult\", \"Adult\"]\n    },\n    \"assignedLicenses\": {\n      \"type\": \"array\",\n      \"description\": \"The licenses assigned\
  \ to the user, including specific disabled service plans. Read-only. Not nullable.\",\n      \"readOnly\": true,\n      \"items\": {\n        \"$ref\": \"#/$defs/assignedLicense\"\n      }\n    },\n    \"assignedPlans\": {\n      \"type\": \"array\",\n      \"description\": \"The plans assigned to the user from subscriptions. Read-only. Not nullable.\",\n      \"readOnly\": true,\n      \"items\": {\n        \"$ref\": \"#/$defs/assignedPlan\"\n      }\n    },\n    \"businessPhones\": {\n      \"type\": \"array\",\n      \"description\": \"The telephone numbers for the user. Only one number can be set for this property. Read-only for users synced from on-premises directory.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"city\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The city where the user is located. Maximum length is 128 characters.\",\n      \"maxLength\": 128\n    },\n    \"companyName\": {\n      \"type\": [\"string\", \"\
  null\"],\n      \"description\": \"The name of the company associated with the user. This property can be useful for describing the company that an external user comes from. Maximum length is 64 characters.\",\n      \"maxLength\": 64\n    },\n    \"consentProvidedForMinor\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Sets whether consent was obtained for minors. Allowed values: null, Granted, Denied, NotRequired.\",\n      \"enum\": [null, \"Granted\", \"Denied\", \"NotRequired\"]\n    },\n    \"country\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The country or region where the user is located. Use the ISO 3166 two-letter country code format (e.g., US, GB, DE). Maximum length is 128 characters.\",\n      \"maxLength\": 128\n    },\n    \"createdDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the user was created in ISO 8601 format and UTC time. Read-only.\"\
  ,\n      \"readOnly\": true\n    },\n    \"creationType\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Indicates whether the user account was created through one of the following methods: as a regular school or work account (null), as an external account (Invitation), as a local account for an Azure Active Directory B2C tenant (LocalAccount), or through self-service sign-up by an internal user using email verification (EmailVerified). Read-only.\",\n      \"readOnly\": true\n    },\n    \"department\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The name of the department in which the user works. Maximum length is 64 characters.\",\n      \"maxLength\": 64\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The name displayed in the address book for the user. This is usually the combination of the first name, middle initial, and last name. This property is required when a user is created and cannot be\
  \ cleared during updates. Maximum length is 256 characters.\",\n      \"maxLength\": 256\n    },\n    \"employeeHireDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the user was hired or will start work in case of a future hire.\"\n    },\n    \"employeeId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The employee identifier assigned to the user by the organization. The maximum length is 16 characters.\",\n      \"maxLength\": 16\n    },\n    \"employeeLeaveDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the user left or will leave the organization.\"\n    },\n    \"employeeOrgData\": {\n      \"description\": \"Represents organization data (e.g., division and costCenter) associated with a user.\",\n      \"$ref\": \"#/$defs/employeeOrgData\"\n    },\n    \"employeeType\": {\n      \"type\"\
  : [\"string\", \"null\"],\n      \"description\": \"Captures enterprise worker type. For example, Employee, Contractor, Consultant, or Vendor.\"\n    },\n    \"externalUserState\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"For an external user invited to the tenant, this property represents the invited user's invitation status. Possible values: PendingAcceptance, Accepted, null. Read-only.\",\n      \"readOnly\": true,\n      \"enum\": [null, \"PendingAcceptance\", \"Accepted\"]\n    },\n    \"externalUserStateChangeDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Shows the timestamp for the latest change to the externalUserState property. Read-only.\",\n      \"readOnly\": true\n    },\n    \"faxNumber\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The fax number of the user.\"\n    },\n    \"givenName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\"\
  : \"The given name (first name) of the user. Maximum length is 64 characters.\",\n      \"maxLength\": 64\n    },\n    \"identities\": {\n      \"type\": \"array\",\n      \"description\": \"Represents the identities that can be used to sign in to this user account. An identity can be provided by Microsoft, by organizations, or by social identity providers. May contain multiple items with the same signInType value.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/objectIdentity\"\n      }\n    },\n    \"imAddresses\": {\n      \"type\": \"array\",\n      \"description\": \"The instant message voice-over-IP (VOIP) session initiation protocol (SIP) addresses for the user. Read-only.\",\n      \"readOnly\": true,\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"isResourceAccount\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Do not use. Reserved for future use.\"\n    },\n    \"jobTitle\": {\n      \"type\": [\"string\", \"null\"],\n \
  \     \"description\": \"The user's job title. Maximum length is 128 characters.\",\n      \"maxLength\": 128\n    },\n    \"lastPasswordChangeDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The time when this Azure AD user last changed their password or when their password was created. Read-only.\",\n      \"readOnly\": true\n    },\n    \"legalAgeGroupClassification\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Used by enterprise applications to determine the legal age group of the user. Read-only.\",\n      \"readOnly\": true,\n      \"enum\": [null, \"MinorWithOutParentalConsent\", \"MinorWithParentalConsent\", \"MinorNoParentalConsentRequired\", \"NotAdult\", \"Adult\"]\n    },\n    \"licenseAssignmentStates\": {\n      \"type\": \"array\",\n      \"description\": \"State of license assignments for this user. Read-only.\",\n      \"readOnly\": true,\n      \"items\": {\n        \"$ref\": \"\
  #/$defs/licenseAssignmentState\"\n      }\n    },\n    \"mail\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"email\",\n      \"description\": \"The SMTP address for the user (e.g., admin@contoso.com). Changes to this property also update the user's proxyAddresses collection to include the value as an SMTP address. This property cannot contain accent characters.\"\n    },\n    \"mailNickname\": {\n      \"type\": \"string\",\n      \"description\": \"The mail alias for the user. This property must be specified when a user is created. Maximum length is 64 characters.\",\n      \"maxLength\": 64\n    },\n    \"mobilePhone\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The primary cellular telephone number for the user. Read-only for users synced from on-premises directory.\"\n    },\n    \"officeLocation\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The office location in the user's place of business.\"\n    },\n    \"\
  onPremisesDistinguishedName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Contains the on-premises Active Directory distinguished name or DN. Read-only.\",\n      \"readOnly\": true\n    },\n    \"onPremisesDomainName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Contains the on-premises domainFQDN, also called dnsDomainName, synced from the on-premises directory. Read-only.\",\n      \"readOnly\": true\n    },\n    \"onPremisesExtensionAttributes\": {\n      \"description\": \"Contains extensionAttributes1-15 for the user. These extension attributes are also known as Exchange custom attributes. Read-only for cloud-only users.\",\n      \"$ref\": \"#/$defs/onPremisesExtensionAttributes\"\n    },\n    \"onPremisesImmutableId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"This property is used to associate an on-premises Active Directory user account to their Azure AD user object. This property must be specified\
  \ when creating a new user if you are using a federated domain for the userPrincipalName (UPN).\"\n    },\n    \"onPremisesLastSyncDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Indicates the last time at which the object was synced with the on-premises directory. Read-only.\",\n      \"readOnly\": true\n    },\n    \"onPremisesProvisioningErrors\": {\n      \"type\": \"array\",\n      \"description\": \"Errors when using Microsoft synchronization product during provisioning. Read-only.\",\n      \"readOnly\": true,\n      \"items\": {\n        \"$ref\": \"#/$defs/onPremisesProvisioningError\"\n      }\n    },\n    \"onPremisesSamAccountName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Contains the on-premises samAccountName synced from the on-premises directory. Read-only.\",\n      \"readOnly\": true\n    },\n    \"onPremisesSecurityIdentifier\": {\n      \"type\": [\"string\", \"null\"],\n\
  \      \"description\": \"Contains the on-premises security identifier (SID) for the user that was synced from on-premises to the cloud. Read-only.\",\n      \"readOnly\": true\n    },\n    \"onPremisesSyncEnabled\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"True if this user object is currently being synced from an on-premises Active Directory (AD); otherwise, the user isn't being synced and can be managed in Azure Active Directory. Read-only.\",\n      \"readOnly\": true\n    },\n    \"onPremisesUserPrincipalName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Contains the on-premises userPrincipalName synced from the on-premises directory. Read-only.\",\n      \"readOnly\": true\n    },\n    \"otherMails\": {\n      \"type\": \"array\",\n      \"description\": \"A list of additional email addresses for the user (e.g., [\\\"bob@contoso.com\\\", \\\"Robert@fabrikam.com\\\"]).\",\n      \"items\": {\n        \"type\": \"string\",\n  \
  \      \"format\": \"email\"\n      }\n    },\n    \"passwordPolicies\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Specifies password policies for the user. This value is an enumeration with one possible value being DisableStrongPassword, which allows weaker passwords than the default policy to be specified. DisablePasswordExpiration can also be specified. The two may be specified together; for example: DisablePasswordExpiration, DisableStrongPassword.\"\n    },\n    \"passwordProfile\": {\n      \"description\": \"Specifies the password profile for the user. The profile contains the user's password. This property is required when a user is created.\",\n      \"$ref\": \"#/$defs/passwordProfile\"\n    },\n    \"postalCode\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The postal code for the user's postal address. The postal code is specific to the user's country/region. Maximum length is 40 characters.\",\n      \"maxLength\": 40\n \
  \   },\n    \"preferredLanguage\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The preferred language for the user, expressed in ISO 639-1 code format (e.g., en-US).\"\n    },\n    \"preferredDataLocation\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The preferred data location for the user, indicating the geographic region for their data.\"\n    },\n    \"provisionedPlans\": {\n      \"type\": \"array\",\n      \"description\": \"The plans that are provisioned for the user. Read-only. Not nullable.\",\n      \"readOnly\": true,\n      \"items\": {\n        \"$ref\": \"#/$defs/provisionedPlan\"\n      }\n    },\n    \"proxyAddresses\": {\n      \"type\": \"array\",\n      \"description\": \"A list that includes the user's SMTP and SIP proxy addresses. For example: [\\\"SMTP:bob@contoso.com\\\", \\\"smtp:bob@sales.contoso.com\\\"]. The address prefixed with SMTP (uppercase) is the primary. Read-only.\",\n      \"readOnly\": true,\n    \
  \  \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"securityIdentifier\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Security identifier (SID) of the user, used in Windows scenarios. Read-only.\",\n      \"readOnly\": true\n    },\n    \"showInAddressList\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Do not use in Microsoft Graph. Manage this property through the Microsoft 365 admin center instead.\"\n    },\n    \"signInActivity\": {\n      \"description\": \"Get the last signed-in date and request ID of the sign-in for a given user. Read-only. Requires Azure AD Premium P1 or P2 license.\",\n      \"readOnly\": true,\n      \"$ref\": \"#/$defs/signInActivity\"\n    },\n    \"signInSessionsValidFromDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Any refresh tokens or sessions tokens (session cookies) issued before this time are invalid, and applications\
  \ will get an error when using an invalid refresh or sessions token to acquire a delegated access token. Read-only.\",\n      \"readOnly\": true\n    },\n    \"state\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The state or province in the user's address. Maximum length is 128 characters.\",\n      \"maxLength\": 128\n    },\n    \"streetAddress\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The street address of the user's place of business. Maximum length is 1024 characters.\",\n      \"maxLength\": 1024\n    },\n    \"surname\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The user's surname (family name or last name). Maximum length is 64 characters.\",\n      \"maxLength\": 64\n    },\n    \"usageLocation\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A two-letter country code (ISO standard 3166). Required for users that will be assigned licenses due to legal requirements to check\
  \ for availability of services in countries/regions. Examples include US, JP, and GB. Not nullable.\",\n      \"pattern\": \"^[A-Z]{2}$\"\n    },\n    \"userPrincipalName\": {\n      \"type\": \"string\",\n      \"description\": \"The user principal name (UPN) of the user. The UPN is an Internet-style sign-in name based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant's verified domain collection. This property is required when a user is created.\",\n      \"format\": \"email\"\n    },\n    \"userType\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A string value that can be used to classify user types in your directory, such as Member and Guest.\",\n      \"enum\": [null, \"Member\", \"Guest\"]\n    }\n  },\n  \"$defs\": {\n    \"assignedLicense\": {\n      \"type\": \"object\",\n      \"description\": \"Represents a license assigned to a user,\
  \ specifying the SKU and any disabled plans.\",\n      \"properties\": {\n        \"disabledPlans\": {\n          \"type\": \"array\",\n          \"description\": \"A collection of the unique identifiers for plans that have been disabled.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          }\n        },\n        \"skuId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier for the SKU.\"\n        }\n      }\n    },\n    \"assignedPlan\": {\n      \"type\": \"object\",\n      \"description\": \"Represents a plan assigned to a user through a subscription.\",\n      \"properties\": {\n        \"assignedDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time at which the plan was assigned.\"\n        },\n        \"capabilityStatus\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Condition of the capability assignment.\",\n          \"enum\": [\"Enabled\", \"Warning\", \"Suspended\", \"Deleted\", \"LockedOut\"]\n        },\n        \"service\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the service (e.g., exchange, SharePoint).\"\n        },\n        \"servicePlanId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"A GUID that identifies the service plan.\"\n        }\n      }\n    },\n    \"employeeOrgData\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Represents organization data associated with a user.\",\n      \"properties\": {\n        \"costCenter\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The cost center associated with the user.\"\n        },\n        \"division\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The name of the division in which the user works.\"\n        }\n\
  \      }\n    },\n    \"objectIdentity\": {\n      \"type\": \"object\",\n      \"description\": \"Represents an identity used to sign in to a user account.\",\n      \"properties\": {\n        \"signInType\": {\n          \"type\": \"string\",\n          \"description\": \"Specifies the user sign-in types in your directory, such as emailAddress, userName, federated, or userPrincipalName.\"\n        },\n        \"issuer\": {\n          \"type\": \"string\",\n          \"description\": \"Specifies the issuer of the identity (e.g., contoso.com for federated identities, or the tenant name for local accounts).\"\n        },\n        \"issuerAssignedId\": {\n          \"type\": \"string\",\n          \"description\": \"Specifies the unique value associated with the identity issued by the issuer. The combination of issuer and issuerAssignedId must be unique.\"\n        }\n      }\n    },\n    \"licenseAssignmentState\": {\n      \"type\": \"object\",\n      \"description\": \"Provides details\
  \ about license assignments.\",\n      \"properties\": {\n        \"assignedByGroup\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uuid\",\n          \"description\": \"The id of the group that assigns this license. If the assignment is a direct-assigned license, this field will be null.\"\n        },\n        \"disabledPlans\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          }\n        },\n        \"error\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"License assignment failure error.\"\n        },\n        \"lastUpdatedDateTime\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date-time\"\n        },\n        \"skuId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"enum\": [\"Active\", \"ActiveWithError\", \"Disabled\"\
  , \"Error\"]\n        }\n      }\n    },\n    \"onPremisesExtensionAttributes\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Contains 15 custom extension attribute properties (extensionAttribute1 through extensionAttribute15). These attributes are synced from on-premises AD for hybrid users.\",\n      \"properties\": {\n        \"extensionAttribute1\": { \"type\": [\"string\", \"null\"] },\n        \"extensionAttribute2\": { \"type\": [\"string\", \"null\"] },\n        \"extensionAttribute3\": { \"type\": [\"string\", \"null\"] },\n        \"extensionAttribute4\": { \"type\": [\"string\", \"null\"] },\n        \"extensionAttribute5\": { \"type\": [\"string\", \"null\"] },\n        \"extensionAttribute6\": { \"type\": [\"string\", \"null\"] },\n        \"extensionAttribute7\": { \"type\": [\"string\", \"null\"] },\n        \"extensionAttribute8\": { \"type\": [\"string\", \"null\"] },\n        \"extensionAttribute9\": { \"type\": [\"string\", \"null\"] },\n    \
  \    \"extensionAttribute10\": { \"type\": [\"string\", \"null\"] },\n        \"extensionAttribute11\": { \"type\": [\"string\", \"null\"] },\n        \"extensionAttribute12\": { \"type\": [\"string\", \"null\"] },\n        \"extensionAttribute13\": { \"type\": [\"string\", \"null\"] },\n        \"extensionAttribute14\": { \"type\": [\"string\", \"null\"] },\n        \"extensionAttribute15\": { \"type\": [\"string\", \"null\"] }\n      }\n    },\n    \"onPremisesProvisioningError\": {\n      \"type\": \"object\",\n      \"description\": \"Represents errors encountered during directory synchronization.\",\n      \"properties\": {\n        \"category\": {\n          \"type\": \"string\",\n          \"description\": \"Category of the provisioning error.\"\n        },\n        \"occurredDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"propertyCausingError\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the\
  \ directory property causing the error.\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"Value of the property causing the error.\"\n        }\n      }\n    },\n    \"passwordProfile\": {\n      \"type\": \"object\",\n      \"description\": \"Contains the password profile associated with a user, including the password itself and policies for password changes.\",\n      \"required\": [\"password\"],\n      \"properties\": {\n        \"forceChangePasswordNextSignIn\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, at next sign-in, the user must change their password. After a password change, this property is automatically reset to false.\",\n          \"default\": false\n        },\n        \"forceChangePasswordNextSignInWithMfa\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, at next sign-in, the user must perform multi-factor authentication (MFA) before being forced to change their\
  \ password.\",\n          \"default\": false\n        },\n        \"password\": {\n          \"type\": \"string\",\n          \"description\": \"The password for the user. This property is required when creating a user. It can be updated, but the user will be required to change the password on the next sign-in. The password must satisfy minimum requirements as specified by the tenant's password complexity policy. By default, a strong password is required.\"\n        }\n      }\n    },\n    \"provisionedPlan\": {\n      \"type\": \"object\",\n      \"description\": \"Represents a service plan that has been provisioned for a user.\",\n      \"properties\": {\n        \"capabilityStatus\": {\n          \"type\": \"string\",\n          \"description\": \"Condition of the capability assignment.\",\n          \"enum\": [\"Enabled\", \"Warning\", \"Suspended\", \"Deleted\", \"LockedOut\"]\n        },\n        \"provisioningStatus\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The provisioning status of the plan.\"\n        },\n        \"service\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the service.\"\n        }\n      }\n    },\n    \"signInActivity\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Provides the last interactive and non-interactive sign-in date and request ID for a specific user.\",\n      \"properties\": {\n        \"lastSignInDateTime\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date-time\",\n          \"description\": \"The last interactive sign-in date and time for a specific user.\"\n        },\n        \"lastSignInRequestId\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Request identifier of the last interactive sign-in performed by this user.\"\n        },\n        \"lastNonInteractiveSignInDateTime\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date-time\",\n          \"description\"\
  : \"The last non-interactive sign-in date for a specific user.\"\n        },\n        \"lastNonInteractiveSignInRequestId\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Request identifier of the last non-interactive sign-in performed by this user.\"\n        }\n      }\n    }\n  },\n  \"examples\": [\n    {\n      \"id\": \"87d349ed-44d7-43e1-9a83-5f2406dee5bd\",\n      \"displayName\": \"Adele Vance\",\n      \"givenName\": \"Adele\",\n      \"surname\": \"Vance\",\n      \"userPrincipalName\": \"adelev@contoso.com\",\n      \"mail\": \"adelev@contoso.com\",\n      \"mailNickname\": \"adelev\",\n      \"accountEnabled\": true,\n      \"jobTitle\": \"Retail Manager\",\n      \"department\": \"Retail\",\n      \"city\": \"Seattle\",\n      \"state\": \"WA\",\n      \"country\": \"US\",\n      \"usageLocation\": \"US\",\n      \"userType\": \"Member\",\n      \"businessPhones\": [\"+1 425 555 0100\"],\n      \"mobilePhone\": \"+1 425 555 0101\",\n      \"\
  officeLocation\": \"Building 18/2111\",\n      \"preferredLanguage\": \"en-US\",\n      \"createdDateTime\": \"2023-06-15T08:00:00Z\"\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-active-directory/refs/heads/main/json-schema/azure-active-directory-user-schema.json
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
title: Azure Active Directory User
---
