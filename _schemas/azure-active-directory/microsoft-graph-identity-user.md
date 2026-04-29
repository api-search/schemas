---
description: Represents an Azure AD user account. Inherits from directoryObject. Contains identity, profile, organizational, and authentication properties.
layout: schema
name: User
properties_list:
- description: True if the account is enabled; otherwise, false.
  name: accountEnabled
  type: boolean
- description: The licenses that are assigned to the user.
  name: assignedLicenses
  type: array
- description: The plans that are assigned to the user.
  name: assignedPlans
  type: array
- description: The telephone numbers for the user.
  name: businessPhones
  type: array
- description: The city where the user is located.
  name: city
  type: '[''string'', ''null'']'
- description: The company name associated with the user.
  name: companyName
  type: '[''string'', ''null'']'
- description: The country or region where the user is located.
  name: country
  type: '[''string'', ''null'']'
- description: The date and time the user was created.
  name: createdDateTime
  type: string
- description: The department in which the user works.
  name: department
  type: '[''string'', ''null'']'
- description: The name displayed in the address book for the user. Required on creation.
  name: displayName
  type: string
- description: The employee identifier assigned to the user by the organization.
  name: employeeId
  type: '[''string'', ''null'']'
- description: Captures the enterprise worker type. For example, Employee, Contractor, Consultant, or Vendor.
  name: employeeType
  type: '[''string'', ''null'']'
- description: The given name (first name) of the user.
  name: givenName
  type: '[''string'', ''null'']'
- description: The user's job title.
  name: jobTitle
  type: '[''string'', ''null'']'
- description: The SMTP address for the user.
  name: mail
  type: '[''string'', ''null'']'
- description: The mail alias for the user. Required on creation.
  name: mailNickname
  type: string
- description: The primary cellular telephone number for the user.
  name: mobilePhone
  type: '[''string'', ''null'']'
- description: The office location in the user's place of business.
  name: officeLocation
  type: '[''string'', ''null'']'
- description: The on-premises Active Directory distinguished name.
  name: onPremisesDistinguishedName
  type: '[''string'', ''null'']'
- description: The on-premises domain name.
  name: onPremisesDomainName
  type: '[''string'', ''null'']'
- description: Used to associate an on-premises Active Directory user account to the Azure AD user object.
  name: onPremisesImmutableId
  type: '[''string'', ''null'']'
- description: The last time at which the object was synced with the on-premises directory.
  name: onPremisesLastSyncDateTime
  type: '[''string'', ''null'']'
- description: True if this user object is currently being synced from an on-premises Active Directory.
  name: onPremisesSyncEnabled
  type: '[''boolean'', ''null'']'
- description: Additional email addresses for the user.
  name: otherMails
  type: array
- description: Specifies password policies for the user. One of DisableStrongPassword and DisablePasswordExpiration, or both.
  name: passwordPolicies
  type: '[''string'', ''null'']'
- description: The postal code for the user's postal address.
  name: postalCode
  type: '[''string'', ''null'']'
- description: 'The preferred language for the user in ISO 639-1 code format. Example: en-US.'
  name: preferredLanguage
  type: '[''string'', ''null'']'
- description: 'The proxy addresses for the user. Example: SMTP:user@contoso.com, smtp:alias@contoso.com.'
  name: proxyAddresses
  type: array
- description: Any refresh tokens or session tokens issued before this time are invalid.
  name: signInSessionsValidFromDateTime
  type: string
- description: The state or province in the user's address.
  name: state
  type: '[''string'', ''null'']'
- description: The street address of the user's place of business.
  name: streetAddress
  type: '[''string'', ''null'']'
- description: The user's surname (family name or last name).
  name: surname
  type: '[''string'', ''null'']'
- description: A two-letter country code (ISO 3166). Required for users who will be assigned licenses.
  name: usageLocation
  type: '[''string'', ''null'']'
- description: 'The user principal name (UPN) of the user. Required on creation. Format: alias@domain.'
  name: userPrincipalName
  type: string
- description: A string value that classifies the user. Typically Member or Guest.
  name: userType
  type: '[''string'', ''null'']'
provider_name: Azure Active Directory
provider_slug: azure-active-directory
schema_file: json-schema/microsoft-graph-identity-user-schema.json
slug: microsoft-graph-identity-user
source_filename: microsoft-graph-identity-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"User\",\n  \"type\": \"object\",\n  \"description\": \"Represents an Azure AD user account. Inherits from directoryObject. Contains identity, profile, organizational, and authentication properties.\",\n  \"properties\": {\n    \"accountEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the account is enabled; otherwise, false.\"\n    },\n    \"assignedLicenses\": {\n      \"type\": \"array\",\n      \"description\": \"The licenses that are assigned to the user.\"\n    },\n    \"assignedPlans\": {\n      \"type\": \"array\",\n      \"description\": \"The plans that are assigned to the user.\"\n    },\n    \"businessPhones\": {\n      \"type\": \"array\",\n      \"description\": \"The telephone numbers for the user.\"\n    },\n    \"city\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The city where the user is located.\"\n    },\n    \"companyName\"\
  : {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The company name associated with the user.\"\n    },\n    \"country\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The country or region where the user is located.\"\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the user was created.\"\n    },\n    \"department\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The department in which the user works.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The name displayed in the address book for the user. Required on creation.\"\n    },\n    \"employeeId\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The employee identifier assigned to the user by the organization.\"\n    },\n    \"employeeType\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Captures the enterprise worker type.\
  \ For example, Employee, Contractor, Consultant, or Vendor.\"\n    },\n    \"givenName\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The given name (first name) of the user.\"\n    },\n    \"jobTitle\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The user's job title.\"\n    },\n    \"mail\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The SMTP address for the user.\"\n    },\n    \"mailNickname\": {\n      \"type\": \"string\",\n      \"description\": \"The mail alias for the user. Required on creation.\"\n    },\n    \"mobilePhone\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The primary cellular telephone number for the user.\"\n    },\n    \"officeLocation\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The office location in the user's place of business.\"\n    },\n    \"onPremisesDistinguishedName\": {\n      \"type\": \"['string', 'null']\",\n      \"description\"\
  : \"The on-premises Active Directory distinguished name.\"\n    },\n    \"onPremisesDomainName\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The on-premises domain name.\"\n    },\n    \"onPremisesImmutableId\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Used to associate an on-premises Active Directory user account to the Azure AD user object.\"\n    },\n    \"onPremisesLastSyncDateTime\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The last time at which the object was synced with the on-premises directory.\"\n    },\n    \"onPremisesSyncEnabled\": {\n      \"type\": \"['boolean', 'null']\",\n      \"description\": \"True if this user object is currently being synced from an on-premises Active Directory.\"\n    },\n    \"otherMails\": {\n      \"type\": \"array\",\n      \"description\": \"Additional email addresses for the user.\"\n    },\n    \"passwordPolicies\": {\n      \"type\": \"['string', 'null']\"\
  ,\n      \"description\": \"Specifies password policies for the user. One of DisableStrongPassword and DisablePasswordExpiration, or both.\"\n    },\n    \"postalCode\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The postal code for the user's postal address.\"\n    },\n    \"preferredLanguage\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The preferred language for the user in ISO 639-1 code format. Example: en-US.\"\n    },\n    \"proxyAddresses\": {\n      \"type\": \"array\",\n      \"description\": \"The proxy addresses for the user. Example: SMTP:user@contoso.com, smtp:alias@contoso.com.\"\n    },\n    \"signInSessionsValidFromDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Any refresh tokens or session tokens issued before this time are invalid.\"\n    },\n    \"state\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The state or province in the user's address.\"\n    },\n    \"streetAddress\"\
  : {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The street address of the user's place of business.\"\n    },\n    \"surname\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The user's surname (family name or last name).\"\n    },\n    \"usageLocation\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"A two-letter country code (ISO 3166). Required for users who will be assigned licenses.\"\n    },\n    \"userPrincipalName\": {\n      \"type\": \"string\",\n      \"description\": \"The user principal name (UPN) of the user. Required on creation. Format: alias@domain.\"\n    },\n    \"userType\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"A string value that classifies the user. Typically Member or Guest.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-user-schema.json
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
title: User
---
