---
description: Schema representing a customer record in Oracle E-Business Suite Trading Community Architecture (TCA). Maps to HZ_PARTIES, HZ_CUST_ACCOUNTS, HZ_PARTY_SITES, HZ_CUST_ACCT_SITES_ALL, and HZ_CUST_SITE_USES_ALL tables. TCA provides a unified model for managing customer, supplier, and partner data.
layout: schema
name: Oracle EBS Customer
properties_list:
- description: Party identifier (HZ_PARTIES.PARTY_ID)
  name: partyId
  type: integer
- description: Party number (system-generated unique identifier)
  name: partyNumber
  type: string
- description: Party name (organization name or person full name)
  name: partyName
  type: string
- description: Party type
  name: partyType
  type: string
- description: Customer category code
  name: category
  type:
  - string
  - 'null'
- description: Party status
  name: status
  type: string
- description: Organization profile (when partyType is ORGANIZATION)
  name: organizationProfile
  type: object
- description: Person profile (when partyType is PERSON)
  name: personProfile
  type: object
- description: Customer accounts associated with this party
  name: customerAccounts
  type: array
- description: Party site/address records
  name: partySites
  type: array
- description: Contact points (phone, email, web, etc.)
  name: contactPoints
  type: array
- description: Party relationships (contacts, hierarchies)
  name: relationships
  type: array
- description: DUNS number
  name: dunsBNumber
  type:
  - string
  - 'null'
- description: Tax identification number
  name: taxPayerIdentificationNumber
  type:
  - string
  - 'null'
- description: Fiscal code (localization)
  name: jgzzFiscalCode
  type:
  - string
  - 'null'
- description: Website URL
  name: url
  type:
  - string
  - 'null'
- description: Primary email address
  name: emailAddress
  type:
  - string
  - 'null'
- description: Primary phone number
  name: primaryPhoneNumber
  type:
  - string
  - 'null'
- description: ''
  name: createdBy
  type: integer
- description: ''
  name: creationDate
  type: string
- description: ''
  name: lastUpdatedBy
  type: integer
- description: ''
  name: lastUpdateDate
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/customer.json
slug: customer
source_filename: customer.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.oracle.com/ebs/customer.json\",\n  \"title\": \"Oracle EBS Customer\",\n  \"description\": \"Schema representing a customer record in Oracle E-Business Suite Trading Community Architecture (TCA). Maps to HZ_PARTIES, HZ_CUST_ACCOUNTS, HZ_PARTY_SITES, HZ_CUST_ACCT_SITES_ALL, and HZ_CUST_SITE_USES_ALL tables. TCA provides a unified model for managing customer, supplier, and partner data.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"partyId\",\n    \"partyName\",\n    \"partyType\"\n  ],\n  \"properties\": {\n    \"partyId\": {\n      \"type\": \"integer\",\n      \"description\": \"Party identifier (HZ_PARTIES.PARTY_ID)\"\n    },\n    \"partyNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Party number (system-generated unique identifier)\",\n      \"maxLength\": 30\n    },\n    \"partyName\": {\n      \"type\": \"string\",\n      \"description\": \"Party\
  \ name (organization name or person full name)\",\n      \"maxLength\": 360\n    },\n    \"partyType\": {\n      \"type\": \"string\",\n      \"description\": \"Party type\",\n      \"enum\": [\n        \"ORGANIZATION\",\n        \"PERSON\",\n        \"PARTY_RELATIONSHIP\",\n        \"GROUP\"\n      ]\n    },\n    \"category\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Customer category code\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Party status\",\n      \"enum\": [\n        \"A\",\n        \"I\"\n      ]\n    },\n    \"organizationProfile\": {\n      \"$ref\": \"#/$defs/OrganizationProfile\",\n      \"description\": \"Organization profile (when partyType is ORGANIZATION)\"\n    },\n    \"personProfile\": {\n      \"$ref\": \"#/$defs/PersonProfile\",\n      \"description\": \"Person profile (when partyType is PERSON)\"\n    },\n    \"customerAccounts\": {\n      \"type\": \"array\",\n      \"description\": \"Customer\
  \ accounts associated with this party\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CustomerAccount\"\n      }\n    },\n    \"partySites\": {\n      \"type\": \"array\",\n      \"description\": \"Party site/address records\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PartySite\"\n      }\n    },\n    \"contactPoints\": {\n      \"type\": \"array\",\n      \"description\": \"Contact points (phone, email, web, etc.)\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ContactPoint\"\n      }\n    },\n    \"relationships\": {\n      \"type\": \"array\",\n      \"description\": \"Party relationships (contacts, hierarchies)\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PartyRelationship\"\n      }\n    },\n    \"dunsBNumber\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"DUNS number\",\n      \"maxLength\": 30\n    },\n    \"taxPayerIdentificationNumber\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Tax identification number\"\
  \n    },\n    \"jgzzFiscalCode\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Fiscal code (localization)\"\n    },\n    \"url\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"Website URL\"\n    },\n    \"emailAddress\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"email\",\n      \"description\": \"Primary email address\"\n    },\n    \"primaryPhoneNumber\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Primary phone number\"\n    },\n    \"createdBy\": {\n      \"type\": \"integer\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"lastUpdatedBy\": {\n      \"type\": \"integer\"\n    },\n    \"lastUpdateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$defs\": {\n    \"OrganizationProfile\": {\n      \"type\": \"object\",\n      \"description\": \"Organization-specific\
  \ profile data (HZ_ORGANIZATION_PROFILES)\",\n      \"properties\": {\n        \"organizationProfileId\": {\n          \"type\": \"integer\",\n          \"description\": \"Organization profile identifier\"\n        },\n        \"organizationName\": {\n          \"type\": \"string\",\n          \"description\": \"Organization legal name\",\n          \"maxLength\": 360\n        },\n        \"knownAs\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Organization known-as/trade name\"\n        },\n        \"duns\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"DUNS number\"\n        },\n        \"sicCode\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Standard Industry Classification code\"\n        },\n        \"sicCodeType\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"SIC code type (SIC, NAICS, etc.)\"\n        },\n        \"employeesTotal\": {\n          \"type\"\
  : [\"integer\", \"null\"],\n          \"description\": \"Total number of employees\"\n        },\n        \"annualRevenue\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Annual revenue\"\n        },\n        \"currencyCode\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Revenue currency code\"\n        },\n        \"yearEstablished\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Year organization was established\"\n        },\n        \"legalStatus\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Legal status (Corporation, Partnership, etc.)\"\n        },\n        \"fiscalYearendMonth\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Fiscal year end month\"\n        },\n        \"lineOfBusiness\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Line of business\"\n        }\n      }\n    },\n    \"PersonProfile\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Person-specific profile data (HZ_PERSON_PROFILES)\",\n      \"properties\": {\n        \"personProfileId\": {\n          \"type\": \"integer\"\n        },\n        \"personTitle\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Title\"\n        },\n        \"personFirstName\": {\n          \"type\": \"string\",\n          \"description\": \"First name\"\n        },\n        \"personMiddleName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Middle name\"\n        },\n        \"personLastName\": {\n          \"type\": \"string\",\n          \"description\": \"Last name\"\n        },\n        \"personNameSuffix\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Name suffix\"\n        },\n        \"gender\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Gender\",\n          \"enum\": [\n            \"MALE\",\n \
  \           \"FEMALE\",\n            null\n          ]\n        },\n        \"dateOfBirth\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\"\n        }\n      }\n    },\n    \"CustomerAccount\": {\n      \"type\": \"object\",\n      \"description\": \"Customer account record (HZ_CUST_ACCOUNTS)\",\n      \"required\": [\n        \"custAccountId\",\n        \"accountNumber\"\n      ],\n      \"properties\": {\n        \"custAccountId\": {\n          \"type\": \"integer\",\n          \"description\": \"Customer account identifier\"\n        },\n        \"accountNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Customer account number\",\n          \"maxLength\": 30\n        },\n        \"accountName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Account name\",\n          \"maxLength\": 240\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Account status\"\
  ,\n          \"enum\": [\n            \"A\",\n            \"I\"\n          ]\n        },\n        \"customerType\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Customer type (R=External, I=Internal)\"\n        },\n        \"customerClassCode\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Customer classification code\"\n        },\n        \"accountEstablishedDate\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\",\n          \"description\": \"Date the account was established\"\n        },\n        \"salesChannelCode\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Sales channel code\"\n        },\n        \"orderTypeId\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Default order type identifier\"\n        },\n        \"priceListId\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Default price list\
  \ identifier\"\n        },\n        \"paymentTermId\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Default payment terms identifier\"\n        },\n        \"creditHold\": {\n          \"type\": \"string\",\n          \"description\": \"Whether account is on credit hold\",\n          \"enum\": [\n            \"Y\",\n            \"N\"\n          ]\n        },\n        \"accountSites\": {\n          \"type\": \"array\",\n          \"description\": \"Customer account sites\",\n          \"items\": {\n            \"$ref\": \"#/$defs/CustomerAccountSite\"\n          }\n        },\n        \"creationDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"lastUpdateDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    },\n    \"CustomerAccountSite\": {\n      \"type\": \"object\",\n      \"description\": \"Customer account site (HZ_CUST_ACCT_SITES_ALL)\",\n      \"\
  properties\": {\n        \"custAcctSiteId\": {\n          \"type\": \"integer\",\n          \"description\": \"Customer account site identifier\"\n        },\n        \"partySiteId\": {\n          \"type\": \"integer\",\n          \"description\": \"Party site identifier\"\n        },\n        \"orgId\": {\n          \"type\": \"integer\",\n          \"description\": \"Operating unit identifier\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"A\",\n            \"I\"\n          ]\n        },\n        \"siteUses\": {\n          \"type\": \"array\",\n          \"description\": \"Site uses (BILL_TO, SHIP_TO, etc.)\",\n          \"items\": {\n            \"$ref\": \"#/$defs/SiteUse\"\n          }\n        }\n      }\n    },\n    \"SiteUse\": {\n      \"type\": \"object\",\n      \"description\": \"Customer site use (HZ_CUST_SITE_USES_ALL)\",\n      \"properties\": {\n        \"siteUseId\": {\n          \"type\": \"integer\",\n     \
  \     \"description\": \"Site use identifier\"\n        },\n        \"siteUseCode\": {\n          \"type\": \"string\",\n          \"description\": \"Site use purpose\",\n          \"enum\": [\n            \"BILL_TO\",\n            \"SHIP_TO\",\n            \"DELIVER_TO\",\n            \"DRAWEE\",\n            \"LEGAL\",\n            \"SOLD_TO\",\n            \"MARKETING\"\n          ]\n        },\n        \"primaryFlag\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Y\",\n            \"N\"\n          ]\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"A\",\n            \"I\"\n          ]\n        },\n        \"locationId\": {\n          \"type\": \"integer\",\n          \"description\": \"Location identifier\"\n        }\n      }\n    },\n    \"PartySite\": {\n      \"type\": \"object\",\n      \"description\": \"Party site/address record (HZ_PARTY_SITES with HZ_LOCATIONS)\",\n      \"required\": [\n \
  \       \"partySiteId\"\n      ],\n      \"properties\": {\n        \"partySiteId\": {\n          \"type\": \"integer\",\n          \"description\": \"Party site identifier\"\n        },\n        \"partySiteNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Party site number\"\n        },\n        \"partySiteName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Party site name\"\n        },\n        \"identifyingAddressFlag\": {\n          \"type\": \"string\",\n          \"description\": \"Whether this is the identifying (primary) address\",\n          \"enum\": [\n            \"Y\",\n            \"N\"\n          ]\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"A\",\n            \"I\"\n          ]\n        },\n        \"location\": {\n          \"$ref\": \"#/$defs/Location\"\n        }\n      }\n    },\n    \"Location\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Physical location/address (HZ_LOCATIONS)\",\n      \"properties\": {\n        \"locationId\": {\n          \"type\": \"integer\",\n          \"description\": \"Location identifier\"\n        },\n        \"address1\": {\n          \"type\": \"string\",\n          \"description\": \"Address line 1\",\n          \"maxLength\": 240\n        },\n        \"address2\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Address line 2\",\n          \"maxLength\": 240\n        },\n        \"address3\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Address line 3\",\n          \"maxLength\": 240\n        },\n        \"address4\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Address line 4\",\n          \"maxLength\": 240\n        },\n        \"city\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"City\",\n          \"maxLength\": 60\n        },\n        \"county\": {\n    \
  \      \"type\": [\"string\", \"null\"],\n          \"description\": \"County\",\n          \"maxLength\": 60\n        },\n        \"state\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"State/province\",\n          \"maxLength\": 60\n        },\n        \"province\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Province\"\n        },\n        \"postalCode\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Postal/ZIP code\",\n          \"maxLength\": 60\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"Country code (ISO 3166-1 alpha-2)\",\n          \"maxLength\": 60\n        }\n      }\n    },\n    \"ContactPoint\": {\n      \"type\": \"object\",\n      \"description\": \"Contact point record (HZ_CONTACT_POINTS)\",\n      \"properties\": {\n        \"contactPointId\": {\n          \"type\": \"integer\",\n          \"description\": \"Contact point\
  \ identifier\"\n        },\n        \"contactPointType\": {\n          \"type\": \"string\",\n          \"description\": \"Contact point type\",\n          \"enum\": [\n            \"PHONE\",\n            \"EMAIL\",\n            \"WEB\",\n            \"EDI\",\n            \"EFT\",\n            \"TLX\"\n          ]\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"A\",\n            \"I\"\n          ]\n        },\n        \"primaryFlag\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Y\",\n            \"N\"\n          ]\n        },\n        \"phoneLineType\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Phone line type (GEN, FAX, MOBILE, PAGER)\",\n          \"enum\": [\n            \"GEN\",\n            \"FAX\",\n            \"MOBILE\",\n            \"PAGER\",\n            null\n          ]\n        },\n        \"phoneCountryCode\": {\n          \"type\": [\"string\", \"null\"\
  ],\n          \"description\": \"Phone country code\"\n        },\n        \"phoneAreaCode\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Phone area code\"\n        },\n        \"phoneNumber\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Phone number\"\n        },\n        \"phoneExtension\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Phone extension\"\n        },\n        \"emailAddress\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"email\",\n          \"description\": \"Email address\"\n        },\n        \"url\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n          \"description\": \"Web URL\"\n        }\n      }\n    },\n    \"PartyRelationship\": {\n      \"type\": \"object\",\n      \"description\": \"Party relationship record (HZ_RELATIONSHIPS)\",\n      \"properties\": {\n        \"relationshipId\": {\n          \"\
  type\": \"integer\"\n        },\n        \"relationshipType\": {\n          \"type\": \"string\",\n          \"description\": \"Relationship type (CONTACT_OF, PARENT_OF, etc.)\"\n        },\n        \"relationshipCode\": {\n          \"type\": \"string\",\n          \"description\": \"Relationship code\"\n        },\n        \"subjectId\": {\n          \"type\": \"integer\",\n          \"description\": \"Subject party identifier\"\n        },\n        \"objectId\": {\n          \"type\": \"integer\",\n          \"description\": \"Object party identifier\"\n        },\n        \"subjectType\": {\n          \"type\": \"string\"\n        },\n        \"objectType\": {\n          \"type\": \"string\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"A\",\n            \"I\"\n          ]\n        },\n        \"startDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"endDate\": {\n          \"\
  type\": [\"string\", \"null\"],\n          \"format\": \"date\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/customer.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: Oracle EBS Customer
---
