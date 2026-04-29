---
description: Schema for SAP business partner master data used across S/4HANA, Business One, and SuccessFactors APIs.
layout: schema
name: SAP Business Partner
properties_list:
- description: Unique business partner number
  name: BusinessPartner
  type: string
- description: 'Category of the business partner: 1=Organization, 2=Person, 3=Group'
  name: BusinessPartnerCategory
  type: string
- description: Full name of the business partner
  name: BusinessPartnerFullName
  type: string
- description: Business partner grouping for number range assignment
  name: BusinessPartnerGrouping
  type: string
- description: First name for person-type business partners
  name: FirstName
  type: string
- description: Last name for person-type business partners
  name: LastName
  type: string
- description: Organization name (line 1) for organization-type business partners
  name: OrganizationBPName1
  type: string
- description: Organization name (line 2)
  name: OrganizationBPName2
  type: string
- description: Primary search term
  name: SearchTerm1
  type: string
- description: Correspondence language (ISO 639-1)
  name: Language
  type: string
- description: Industry sector key
  name: Industry
  type: string
- description: Legal form of the organization
  name: LegalForm
  type: string
- description: Date the business partner record was created
  name: CreationDate
  type: string
- description: Date of last modification
  name: LastChangeDate
  type: string
- description: Whether the business partner is a natural person
  name: IsNaturalPerson
  type: string
- description: Business partner addresses
  name: Addresses
  type: array
- description: Business partner bank account details
  name: BankAccounts
  type: array
- description: Tax identification numbers
  name: TaxNumbers
  type: array
- description: Business partner roles (customer, supplier, etc.)
  name: Roles
  type: array
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-business-partner-schema.json
slug: sap-business-partner
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.sap.com/schemas/sap/business-partner.json\",\n  \"title\": \"SAP Business Partner\",\n  \"description\": \"Schema for SAP business partner master data used across S/4HANA, Business One, and SuccessFactors APIs.\",\n  \"type\": \"object\",\n  \"required\": [\"BusinessPartner\", \"BusinessPartnerCategory\"],\n  \"properties\": {\n    \"BusinessPartner\": {\n      \"type\": \"string\",\n      \"description\": \"Unique business partner number\",\n      \"maxLength\": 10,\n      \"pattern\": \"^[0-9A-Z]+$\"\n    },\n    \"BusinessPartnerCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Category of the business partner: 1=Organization, 2=Person, 3=Group\",\n      \"enum\": [\"1\", \"2\", \"3\"]\n    },\n    \"BusinessPartnerFullName\": {\n      \"type\": \"string\",\n      \"description\": \"Full name of the business partner\",\n      \"maxLength\": 81\n    },\n    \"\
  BusinessPartnerGrouping\": {\n      \"type\": \"string\",\n      \"description\": \"Business partner grouping for number range assignment\",\n      \"maxLength\": 4\n    },\n    \"FirstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name for person-type business partners\",\n      \"maxLength\": 40\n    },\n    \"LastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name for person-type business partners\",\n      \"maxLength\": 40\n    },\n    \"OrganizationBPName1\": {\n      \"type\": \"string\",\n      \"description\": \"Organization name (line 1) for organization-type business partners\",\n      \"maxLength\": 40\n    },\n    \"OrganizationBPName2\": {\n      \"type\": \"string\",\n      \"description\": \"Organization name (line 2)\",\n      \"maxLength\": 40\n    },\n    \"SearchTerm1\": {\n      \"type\": \"string\",\n      \"description\": \"Primary search term\",\n      \"maxLength\": 20\n    },\n    \"Language\": {\n      \"type\":\
  \ \"string\",\n      \"description\": \"Correspondence language (ISO 639-1)\",\n      \"maxLength\": 2,\n      \"pattern\": \"^[A-Z]{2}$\"\n    },\n    \"Industry\": {\n      \"type\": \"string\",\n      \"description\": \"Industry sector key\",\n      \"maxLength\": 10\n    },\n    \"LegalForm\": {\n      \"type\": \"string\",\n      \"description\": \"Legal form of the organization\",\n      \"maxLength\": 2\n    },\n    \"CreationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the business partner record was created\"\n    },\n    \"LastChangeDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of last modification\"\n    },\n    \"IsNaturalPerson\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the business partner is a natural person\",\n      \"enum\": [\"X\", \"\"]\n    },\n    \"Addresses\": {\n      \"type\": \"array\",\n      \"description\": \"Business partner\
  \ addresses\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Address\"\n      }\n    },\n    \"BankAccounts\": {\n      \"type\": \"array\",\n      \"description\": \"Business partner bank account details\",\n      \"items\": {\n        \"$ref\": \"#/$defs/BankAccount\"\n      }\n    },\n    \"TaxNumbers\": {\n      \"type\": \"array\",\n      \"description\": \"Tax identification numbers\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TaxNumber\"\n      }\n    },\n    \"Roles\": {\n      \"type\": \"array\",\n      \"description\": \"Business partner roles (customer, supplier, etc.)\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Role\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"Business partner address record\",\n      \"properties\": {\n        \"AddressID\": {\n          \"type\": \"string\",\n          \"description\": \"Address identifier\"\n        },\n        \"Country\": {\n          \"type\": \"\
  string\",\n          \"description\": \"Country code (ISO 3166-1 alpha-2)\",\n          \"maxLength\": 2,\n          \"pattern\": \"^[A-Z]{2}$\"\n        },\n        \"Region\": {\n          \"type\": \"string\",\n          \"description\": \"Region or state code\",\n          \"maxLength\": 3\n        },\n        \"CityName\": {\n          \"type\": \"string\",\n          \"description\": \"City name\",\n          \"maxLength\": 40\n        },\n        \"PostalCode\": {\n          \"type\": \"string\",\n          \"description\": \"Postal code\",\n          \"maxLength\": 10\n        },\n        \"StreetName\": {\n          \"type\": \"string\",\n          \"description\": \"Street name\",\n          \"maxLength\": 60\n        },\n        \"HouseNumber\": {\n          \"type\": \"string\",\n          \"description\": \"House number\",\n          \"maxLength\": 10\n        }\n      }\n    },\n    \"BankAccount\": {\n      \"type\": \"object\",\n      \"description\": \"Business partner\
  \ bank account details\",\n      \"properties\": {\n        \"BankCountryKey\": {\n          \"type\": \"string\",\n          \"description\": \"Country key of the bank\",\n          \"maxLength\": 2\n        },\n        \"BankNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Bank routing or sort code\",\n          \"maxLength\": 15\n        },\n        \"BankAccount\": {\n          \"type\": \"string\",\n          \"description\": \"Bank account number\",\n          \"maxLength\": 18\n        },\n        \"IBAN\": {\n          \"type\": \"string\",\n          \"description\": \"International Bank Account Number\",\n          \"maxLength\": 34,\n          \"pattern\": \"^[A-Z]{2}[0-9]{2}[A-Z0-9]+$\"\n        },\n        \"SWIFTCode\": {\n          \"type\": \"string\",\n          \"description\": \"SWIFT/BIC code\",\n          \"maxLength\": 11\n        }\n      }\n    },\n    \"TaxNumber\": {\n      \"type\": \"object\",\n      \"description\": \"Tax identification\
  \ number\",\n      \"properties\": {\n        \"BPTaxType\": {\n          \"type\": \"string\",\n          \"description\": \"Tax number category\"\n        },\n        \"BPTaxNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Tax identification number value\"\n        }\n      }\n    },\n    \"Role\": {\n      \"type\": \"object\",\n      \"description\": \"Business partner role assignment\",\n      \"properties\": {\n        \"BusinessPartnerRole\": {\n          \"type\": \"string\",\n          \"description\": \"Role code (e.g., FLCU01=Customer, FLVN01=Vendor)\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-business-partner-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: SAP Business Partner
---
