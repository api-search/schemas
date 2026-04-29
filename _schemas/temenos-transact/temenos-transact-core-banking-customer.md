---
description: A customer record in Temenos Transact representing an individual or corporate entity with a banking relationship.
layout: schema
name: Customer
properties_list:
- description: Unique system-generated customer identifier
  name: customerId
  type: string
- description: Short alphanumeric code identifying the customer (3-10 characters, first character alphabetic)
  name: customerMnemonic
  type: string
- description: Short name of the customer (3-35 characters, uppercase)
  name: shortName
  type: string
- description: Full name entries for the customer
  name: customerNames
  type: array
- description: Display name entries for the customer
  name: displayNames
  type: array
- description: Customer title
  name: title
  type: string
- description: Customer gender
  name: gender
  type: string
- description: Customer date of birth
  name: dateOfBirth
  type: string
- description: Nationality code
  name: nationalityId
  type: string
- description: Country of residence code
  name: residenceId
  type: string
- description: Preferred language code
  name: language
  type: integer
- description: Customer status code (1 = active)
  name: customerStatus
  type: integer
- description: Customer sector classification (1-4 digits)
  name: sectorId
  type: integer
- description: Industry classification code
  name: industryId
  type: integer
- description: Assigned account officer identifier
  name: accountOfficerId
  type: integer
- description: Target market segment
  name: target
  type: integer
- description: Contact communication devices (phone, email)
  name: communicationDevices
  type: array
- description: Customer address records
  name: addresses
  type: array
- description: Company identifier the customer belongs to
  name: customerCompany
  type: string
- description: AML verification check status
  name: amlCheck
  type: string
- description: AML verification result
  name: amlResult
  type: string
- description: KYC compliance status
  name: kycStatus
  type: string
provider_name: Temenos Transact
provider_slug: temenos-transact
schema_file: json-schema/temenos-transact-core-banking-customer-schema.json
slug: temenos-transact-core-banking-customer
source_filename: temenos-transact-core-banking-customer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Customer\",\n  \"type\": \"object\",\n  \"description\": \"A customer record in Temenos Transact representing an individual or corporate entity with a banking relationship.\",\n  \"properties\": {\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique system-generated customer identifier\"\n    },\n    \"customerMnemonic\": {\n      \"type\": \"string\",\n      \"description\": \"Short alphanumeric code identifying the customer (3-10 characters, first character alphabetic)\"\n    },\n    \"shortName\": {\n      \"type\": \"string\",\n      \"description\": \"Short name of the customer (3-35 characters, uppercase)\"\n    },\n    \"customerNames\": {\n      \"type\": \"array\",\n      \"description\": \"Full name entries for the customer\"\n    },\n    \"displayNames\": {\n      \"type\": \"array\",\n      \"description\": \"Display name entries for the customer\"\
  \n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Customer title\"\n    },\n    \"gender\": {\n      \"type\": \"string\",\n      \"description\": \"Customer gender\"\n    },\n    \"dateOfBirth\": {\n      \"type\": \"string\",\n      \"description\": \"Customer date of birth\"\n    },\n    \"nationalityId\": {\n      \"type\": \"string\",\n      \"description\": \"Nationality code\"\n    },\n    \"residenceId\": {\n      \"type\": \"string\",\n      \"description\": \"Country of residence code\"\n    },\n    \"language\": {\n      \"type\": \"integer\",\n      \"description\": \"Preferred language code\"\n    },\n    \"customerStatus\": {\n      \"type\": \"integer\",\n      \"description\": \"Customer status code (1 = active)\"\n    },\n    \"sectorId\": {\n      \"type\": \"integer\",\n      \"description\": \"Customer sector classification (1-4 digits)\"\n    },\n    \"industryId\": {\n      \"type\": \"integer\",\n      \"description\": \"Industry classification\
  \ code\"\n    },\n    \"accountOfficerId\": {\n      \"type\": \"integer\",\n      \"description\": \"Assigned account officer identifier\"\n    },\n    \"target\": {\n      \"type\": \"integer\",\n      \"description\": \"Target market segment\"\n    },\n    \"communicationDevices\": {\n      \"type\": \"array\",\n      \"description\": \"Contact communication devices (phone, email)\"\n    },\n    \"addresses\": {\n      \"type\": \"array\",\n      \"description\": \"Customer address records\"\n    },\n    \"customerCompany\": {\n      \"type\": \"string\",\n      \"description\": \"Company identifier the customer belongs to\"\n    },\n    \"amlCheck\": {\n      \"type\": \"string\",\n      \"description\": \"AML verification check status\"\n    },\n    \"amlResult\": {\n      \"type\": \"string\",\n      \"description\": \"AML verification result\"\n    },\n    \"kycStatus\": {\n      \"type\": \"string\",\n      \"description\": \"KYC compliance status\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/json-schema/temenos-transact-core-banking-customer-schema.json
tags:
- Banking
- Core Banking
- Digital Banking
- Enterprise
- Financial Services
- Fintech
title: Customer
---
