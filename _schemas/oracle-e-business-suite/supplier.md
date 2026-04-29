---
description: Schema representing a supplier/vendor record in Oracle E-Business Suite Purchasing and Payables modules. Maps to AP_SUPPLIERS, AP_SUPPLIER_SITES_ALL, AP_SUPPLIER_CONTACTS, and the Trading Community Architecture (TCA) party model (HZ_PARTIES).
layout: schema
name: Oracle EBS Supplier
properties_list:
- description: Vendor identifier (AP_SUPPLIERS.VENDOR_ID)
  name: vendorId
  type: integer
- description: Vendor name
  name: vendorName
  type: string
- description: Vendor number
  name: segment1
  type: string
- description: Vendor type lookup code (e.g., CONTRACTOR, EMPLOYEE, VENDOR)
  name: vendorType
  type:
  - string
  - 'null'
- description: TCA party identifier (HZ_PARTIES.PARTY_ID)
  name: partyId
  type: integer
- description: Tax payer identification number (EIN/SSN/TIN)
  name: taxPayerId
  type:
  - string
  - 'null'
- description: Tax registration number (VAT number)
  name: taxRegistrationNumber
  type:
  - string
  - 'null'
- description: Standard Industry Classification (SIC) code
  name: standardIndustryClass
  type:
  - string
  - 'null'
- description: DUNS number
  name: dunsBNumber
  type:
  - string
  - 'null'
- description: One-time vendor flag
  name: oneTimeFlag
  type: string
- description: Our customer number at the vendor
  name: customerNum
  type:
  - string
  - 'null'
- description: Minority group classification
  name: minorityGroupLookupCode
  type:
  - string
  - 'null'
- description: Small business flag
  name: smallBusinessFlag
  type: string
- description: Women-owned business flag
  name: womenOwnedFlag
  type: string
- description: Default payment currency code (ISO 4217)
  name: paymentCurrencyCode
  type:
  - string
  - 'null'
- description: Default invoice currency code (ISO 4217)
  name: invoiceCurrencyCode
  type:
  - string
  - 'null'
- description: Default payment method lookup code
  name: paymentMethodCode
  type:
  - string
  - 'null'
- description: Pay group lookup code
  name: payGroupLookupCode
  type:
  - string
  - 'null'
- description: Default payment terms identifier (AP_TERMS.TERM_ID)
  name: termsId
  type:
  - integer
  - 'null'
- description: Default payment terms name
  name: termsName
  type:
  - string
  - 'null'
- description: ''
  name: alwaysTakePrepaymentDiscFlag
  type: string
- description: Pay date basis (DISCOUNT, DUE)
  name: payDateBasisLookupCode
  type:
  - string
  - 'null'
- description: Invoice amount limit
  name: invoiceAmountLimit
  type:
  - number
  - 'null'
- description: Whether all payments are on hold
  name: holdAllPaymentsFlag
  type: string
- description: Whether unmatched invoices are on hold
  name: holdUnmatchedInvoicesFlag
  type: string
- description: Invoice match option
  name: matchOption
  type:
  - string
  - 'null'
- description: Whether the vendor is currently active/enabled
  name: enabled
  type: boolean
- description: Date the vendor becomes active
  name: startDateActive
  type: string
- description: Date the vendor becomes inactive
  name: endDateActive
  type:
  - string
  - 'null'
- description: Vendor site records
  name: sites
  type: array
- description: Vendor contact records
  name: contacts
  type: array
- description: Vendor bank account assignments
  name: bankAccounts
  type: array
- description: User who created the record
  name: createdBy
  type: integer
- description: Record creation date
  name: creationDate
  type: string
- description: User who last updated the record
  name: lastUpdatedBy
  type: integer
- description: Record last update date
  name: lastUpdateDate
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/supplier.json
slug: supplier
source_filename: supplier.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.oracle.com/ebs/supplier.json\",\n  \"title\": \"Oracle EBS Supplier\",\n  \"description\": \"Schema representing a supplier/vendor record in Oracle E-Business Suite Purchasing and Payables modules. Maps to AP_SUPPLIERS, AP_SUPPLIER_SITES_ALL, AP_SUPPLIER_CONTACTS, and the Trading Community Architecture (TCA) party model (HZ_PARTIES).\",\n  \"type\": \"object\",\n  \"required\": [\n    \"vendorId\",\n    \"vendorName\"\n  ],\n  \"properties\": {\n    \"vendorId\": {\n      \"type\": \"integer\",\n      \"description\": \"Vendor identifier (AP_SUPPLIERS.VENDOR_ID)\"\n    },\n    \"vendorName\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor name\",\n      \"maxLength\": 240\n    },\n    \"segment1\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor number\",\n      \"maxLength\": 30\n    },\n    \"vendorType\": {\n      \"type\": [\"string\", \"null\"\
  ],\n      \"description\": \"Vendor type lookup code (e.g., CONTRACTOR, EMPLOYEE, VENDOR)\"\n    },\n    \"partyId\": {\n      \"type\": \"integer\",\n      \"description\": \"TCA party identifier (HZ_PARTIES.PARTY_ID)\"\n    },\n    \"taxPayerId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Tax payer identification number (EIN/SSN/TIN)\",\n      \"maxLength\": 20\n    },\n    \"taxRegistrationNumber\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Tax registration number (VAT number)\"\n    },\n    \"standardIndustryClass\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Standard Industry Classification (SIC) code\",\n      \"maxLength\": 25\n    },\n    \"dunsBNumber\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"DUNS number\",\n      \"maxLength\": 30\n    },\n    \"oneTimeFlag\": {\n      \"type\": \"string\",\n      \"description\": \"One-time vendor flag\",\n      \"enum\": [\n       \
  \ \"Y\",\n        \"N\"\n      ]\n    },\n    \"customerNum\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Our customer number at the vendor\"\n    },\n    \"minorityGroupLookupCode\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Minority group classification\"\n    },\n    \"smallBusinessFlag\": {\n      \"type\": \"string\",\n      \"description\": \"Small business flag\",\n      \"enum\": [\n        \"Y\",\n        \"N\"\n      ]\n    },\n    \"womenOwnedFlag\": {\n      \"type\": \"string\",\n      \"description\": \"Women-owned business flag\",\n      \"enum\": [\n        \"Y\",\n        \"N\"\n      ]\n    },\n    \"paymentCurrencyCode\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Default payment currency code (ISO 4217)\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"invoiceCurrencyCode\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Default invoice currency code (ISO 4217)\"\
  ,\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"paymentMethodCode\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Default payment method lookup code\"\n    },\n    \"payGroupLookupCode\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Pay group lookup code\"\n    },\n    \"termsId\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Default payment terms identifier (AP_TERMS.TERM_ID)\"\n    },\n    \"termsName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Default payment terms name\"\n    },\n    \"alwaysTakePrepaymentDiscFlag\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Y\",\n        \"N\"\n      ]\n    },\n    \"payDateBasisLookupCode\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Pay date basis (DISCOUNT, DUE)\"\n    },\n    \"invoiceAmountLimit\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Invoice amount limit\"\n    },\n\
  \    \"holdAllPaymentsFlag\": {\n      \"type\": \"string\",\n      \"description\": \"Whether all payments are on hold\",\n      \"enum\": [\n        \"Y\",\n        \"N\"\n      ]\n    },\n    \"holdUnmatchedInvoicesFlag\": {\n      \"type\": \"string\",\n      \"description\": \"Whether unmatched invoices are on hold\",\n      \"enum\": [\n        \"Y\",\n        \"N\"\n      ]\n    },\n    \"matchOption\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Invoice match option\",\n      \"enum\": [\n        \"P\",\n        \"R\",\n        null\n      ]\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the vendor is currently active/enabled\"\n    },\n    \"startDateActive\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the vendor becomes active\"\n    },\n    \"endDateActive\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Date\
  \ the vendor becomes inactive\"\n    },\n    \"sites\": {\n      \"type\": \"array\",\n      \"description\": \"Vendor site records\",\n      \"items\": {\n        \"$ref\": \"#/$defs/SupplierSite\"\n      }\n    },\n    \"contacts\": {\n      \"type\": \"array\",\n      \"description\": \"Vendor contact records\",\n      \"items\": {\n        \"$ref\": \"#/$defs/SupplierContact\"\n      }\n    },\n    \"bankAccounts\": {\n      \"type\": \"array\",\n      \"description\": \"Vendor bank account assignments\",\n      \"items\": {\n        \"$ref\": \"#/$defs/VendorBankAccount\"\n      }\n    },\n    \"createdBy\": {\n      \"type\": \"integer\",\n      \"description\": \"User who created the record\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record creation date\"\n    },\n    \"lastUpdatedBy\": {\n      \"type\": \"integer\",\n      \"description\": \"User who last updated the record\"\n    },\n    \"lastUpdateDate\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record last update date\"\n    }\n  },\n  \"$defs\": {\n    \"SupplierSite\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"vendorSiteId\",\n        \"vendorSiteCode\"\n      ],\n      \"description\": \"Vendor site record (AP_SUPPLIER_SITES_ALL)\",\n      \"properties\": {\n        \"vendorSiteId\": {\n          \"type\": \"integer\",\n          \"description\": \"Vendor site identifier\"\n        },\n        \"vendorSiteCode\": {\n          \"type\": \"string\",\n          \"description\": \"Vendor site code (unique within vendor)\",\n          \"maxLength\": 15\n        },\n        \"vendorSiteCodeAlt\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Alternate vendor site code\"\n        },\n        \"addressLine1\": {\n          \"type\": \"string\",\n          \"description\": \"Address line 1\",\n          \"maxLength\": 240\n        },\n \
  \       \"addressLine2\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Address line 2\",\n          \"maxLength\": 240\n        },\n        \"addressLine3\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Address line 3\",\n          \"maxLength\": 240\n        },\n        \"city\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"City\",\n          \"maxLength\": 25\n        },\n        \"state\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"State/province\",\n          \"maxLength\": 150\n        },\n        \"zip\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"ZIP/postal code\",\n          \"maxLength\": 20\n        },\n        \"country\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Country code (ISO 3166-1 alpha-2)\",\n          \"maxLength\": 25\n        },\n        \"province\": {\n          \"\
  type\": [\"string\", \"null\"],\n          \"description\": \"Province\"\n        },\n        \"phone\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Phone number\"\n        },\n        \"fax\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Fax number\"\n        },\n        \"emailAddress\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"email\",\n          \"description\": \"Email address\"\n        },\n        \"purchasingSiteFlag\": {\n          \"type\": \"string\",\n          \"description\": \"Whether this site is used for purchasing\",\n          \"enum\": [\n            \"Y\",\n            \"N\"\n          ]\n        },\n        \"rfqOnlySiteFlag\": {\n          \"type\": \"string\",\n          \"description\": \"Whether this site is only for RFQs\",\n          \"enum\": [\n            \"Y\",\n            \"N\"\n          ]\n        },\n        \"paymentSiteFlag\": {\n          \"type\": \"\
  string\",\n          \"description\": \"Whether this site receives payments\",\n          \"enum\": [\n            \"Y\",\n            \"N\"\n          ]\n        },\n        \"primaryPaymentSiteFlag\": {\n          \"type\": \"string\",\n          \"description\": \"Whether this is the primary payment site\",\n          \"enum\": [\n            \"Y\",\n            \"N\"\n          ]\n        },\n        \"paymentMethodCode\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Site-level payment method override\"\n        },\n        \"termsId\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Site-level payment terms override\"\n        },\n        \"paymentCurrencyCode\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Site-level payment currency\"\n        },\n        \"invoiceCurrencyCode\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Site-level invoice currency\"\n\
  \        },\n        \"shipToLocationId\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Default ship-to location for this site\"\n        },\n        \"billToLocationId\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Default bill-to location for this site\"\n        },\n        \"orgId\": {\n          \"type\": \"integer\",\n          \"description\": \"Operating unit identifier\"\n        },\n        \"inactiveDate\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\",\n          \"description\": \"Date the site becomes inactive\"\n        },\n        \"creationDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"lastUpdateDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    },\n    \"SupplierContact\": {\n      \"type\": \"object\",\n      \"description\": \"Vendor contact record (AP_SUPPLIER_CONTACTS)\"\
  ,\n      \"properties\": {\n        \"vendorContactId\": {\n          \"type\": \"integer\",\n          \"description\": \"Vendor contact identifier\"\n        },\n        \"vendorSiteId\": {\n          \"type\": \"integer\",\n          \"description\": \"Associated vendor site identifier\"\n        },\n        \"personFirstName\": {\n          \"type\": \"string\",\n          \"description\": \"Contact first name\",\n          \"maxLength\": 15\n        },\n        \"personMiddleName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Contact middle name\"\n        },\n        \"personLastName\": {\n          \"type\": \"string\",\n          \"description\": \"Contact last name\",\n          \"maxLength\": 15\n        },\n        \"personTitle\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Contact title\"\n        },\n        \"areaCode\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Phone area\
  \ code\"\n        },\n        \"phone\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Phone number\"\n        },\n        \"emailAddress\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"email\",\n          \"description\": \"Contact email\"\n        },\n        \"department\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Contact department\"\n        },\n        \"inactiveDate\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\"\n        }\n      }\n    },\n    \"VendorBankAccount\": {\n      \"type\": \"object\",\n      \"description\": \"Vendor bank account assignment (IBY_EXT_BANK_ACCOUNTS linked via IBY_PMT_INSTR_USES_ALL)\",\n      \"properties\": {\n        \"instrumentPaymentUseId\": {\n          \"type\": \"integer\",\n          \"description\": \"Payment instrument use identifier\"\n        },\n        \"extBankAccountId\": {\n          \"type\": \"integer\",\n\
  \          \"description\": \"External bank account identifier\"\n        },\n        \"bankName\": {\n          \"type\": \"string\",\n          \"description\": \"Bank name\"\n        },\n        \"bankNumber\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Bank number/routing number\"\n        },\n        \"branchName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Bank branch name\"\n        },\n        \"branchNumber\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Branch number\"\n        },\n        \"bankAccountNum\": {\n          \"type\": \"string\",\n          \"description\": \"Bank account number\"\n        },\n        \"bankAccountName\": {\n          \"type\": \"string\",\n          \"description\": \"Bank account name\"\n        },\n        \"iban\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"IBAN (International Bank Account Number)\"\n       \
  \ },\n        \"currencyCode\": {\n          \"type\": \"string\",\n          \"description\": \"Account currency code\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"Bank country code\"\n        },\n        \"startDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"endDate\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\"\n        },\n        \"primaryFlag\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Y\",\n            \"N\"\n          ]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/supplier.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: Oracle EBS Supplier
---
