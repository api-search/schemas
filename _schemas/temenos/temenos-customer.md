---
description: Schema for Temenos customer records including individual and corporate customers with personal data, addresses, identification documents, KYC status, and relationship information.
layout: schema
name: Temenos Customer
properties_list:
- description: Unique customer identifier assigned by the Temenos system
  name: customerId
  type: string
- description: Classification of the customer
  name: customerType
  type: string
- description: Customer honorific title
  name: title
  type: string
- description: First name for individual customers
  name: firstName
  type: string
- description: Middle name for individual customers
  name: middleName
  type: string
- description: Last name for individual customers or company name for corporate
  name: lastName
  type: string
- description: Company name for corporate customers
  name: companyName
  type: string
- description: Date of birth for individual customers
  name: dateOfBirth
  type:
  - string
  - 'null'
- description: Nationality in ISO 3166-1 alpha-2 format
  name: nationality
  type: string
- description: Country of residence in ISO 3166-1 alpha-2 format
  name: countryOfResidence
  type: string
- description: Preferred language in ISO 639-1 format
  name: language
  type: string
- description: Primary email address
  name: email
  type: string
- description: Primary phone number in E.164 format
  name: phone
  type: string
- description: Know Your Customer verification status
  name: kycStatus
  type: string
- description: Customer risk rating from compliance assessment
  name: riskRating
  type: string
- description: Customer record status
  name: status
  type: string
- description: Date the customer was onboarded
  name: onboardingDate
  type: string
- description: Customer addresses
  name: addresses
  type: array
- description: Identity verification documents
  name: identificationDocuments
  type: array
- description: Customer segmentation category
  name: segment
  type: string
- description: Assigned relationship manager identifier
  name: relationshipManager
  type: string
provider_name: Temenos
provider_slug: temenos
schema_file: json-schema/temenos-customer-schema.json
slug: temenos-customer
source_filename: temenos-customer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://temenos.com/schemas/temenos/customer.json\",\n  \"title\": \"Temenos Customer\",\n  \"description\": \"Schema for Temenos customer records including individual and corporate customers with personal data, addresses, identification documents, KYC status, and relationship information.\",\n  \"type\": \"object\",\n  \"required\": [\"customerId\", \"customerType\", \"status\"],\n  \"properties\": {\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique customer identifier assigned by the Temenos system\"\n    },\n    \"customerType\": {\n      \"type\": \"string\",\n      \"description\": \"Classification of the customer\",\n      \"enum\": [\"INDIVIDUAL\", \"CORPORATE\"]\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Customer honorific title\",\n      \"enum\": [\"Mr\", \"Mrs\", \"Ms\", \"Dr\", \"Prof\"]\n    },\n    \"firstName\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"First name for individual customers\",\n      \"maxLength\": 100\n    },\n    \"middleName\": {\n      \"type\": \"string\",\n      \"description\": \"Middle name for individual customers\",\n      \"maxLength\": 100\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name for individual customers or company name for corporate\",\n      \"maxLength\": 200\n    },\n    \"companyName\": {\n      \"type\": \"string\",\n      \"description\": \"Company name for corporate customers\",\n      \"maxLength\": 200\n    },\n    \"dateOfBirth\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Date of birth for individual customers\"\n    },\n    \"nationality\": {\n      \"type\": \"string\",\n      \"description\": \"Nationality in ISO 3166-1 alpha-2 format\",\n      \"pattern\": \"^[A-Z]{2}$\"\n    },\n    \"countryOfResidence\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Country of residence in ISO 3166-1 alpha-2 format\",\n      \"pattern\": \"^[A-Z]{2}$\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Preferred language in ISO 639-1 format\",\n      \"pattern\": \"^[a-z]{2}$\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Primary email address\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Primary phone number in E.164 format\",\n      \"pattern\": \"^\\\\+[1-9][0-9]{1,14}$\"\n    },\n    \"kycStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Know Your Customer verification status\",\n      \"enum\": [\"VERIFIED\", \"PENDING\", \"REJECTED\", \"EXPIRED\", \"NOT_STARTED\"]\n    },\n    \"riskRating\": {\n      \"type\": \"string\",\n      \"description\": \"Customer risk rating from compliance assessment\",\n      \"enum\": [\"LOW\", \"MEDIUM\", \"HIGH\", \"VERY_HIGH\"\
  ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Customer record status\",\n      \"enum\": [\"ACTIVE\", \"INACTIVE\", \"CLOSED\", \"SUSPENDED\"]\n    },\n    \"onboardingDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the customer was onboarded\"\n    },\n    \"addresses\": {\n      \"type\": \"array\",\n      \"description\": \"Customer addresses\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Address\"\n      }\n    },\n    \"identificationDocuments\": {\n      \"type\": \"array\",\n      \"description\": \"Identity verification documents\",\n      \"items\": {\n        \"$ref\": \"#/$defs/IdentificationDocument\"\n      }\n    },\n    \"segment\": {\n      \"type\": \"string\",\n      \"description\": \"Customer segmentation category\"\n    },\n    \"relationshipManager\": {\n      \"type\": \"string\",\n      \"description\": \"Assigned relationship manager identifier\"\n    }\n  },\n  \"$defs\"\
  : {\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"Physical or mailing address\",\n      \"required\": [\"addressType\", \"country\"],\n      \"properties\": {\n        \"addressType\": {\n          \"type\": \"string\",\n          \"description\": \"Type of address\",\n          \"enum\": [\"RESIDENTIAL\", \"BUSINESS\", \"CORRESPONDENCE\", \"REGISTERED\"]\n        },\n        \"addressLine1\": {\n          \"type\": \"string\",\n          \"description\": \"First line of the address\",\n          \"maxLength\": 200\n        },\n        \"addressLine2\": {\n          \"type\": \"string\",\n          \"description\": \"Second line of the address\",\n          \"maxLength\": 200\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"City name\",\n          \"maxLength\": 100\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"State, province, or region\",\n          \"maxLength\"\
  : 100\n        },\n        \"postalCode\": {\n          \"type\": \"string\",\n          \"description\": \"Postal or zip code\",\n          \"maxLength\": 20\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"Country in ISO 3166-1 alpha-2 format\",\n          \"pattern\": \"^[A-Z]{2}$\"\n        }\n      }\n    },\n    \"IdentificationDocument\": {\n      \"type\": \"object\",\n      \"description\": \"Identity verification document\",\n      \"required\": [\"documentType\", \"documentNumber\"],\n      \"properties\": {\n        \"documentType\": {\n          \"type\": \"string\",\n          \"description\": \"Type of identification document\",\n          \"enum\": [\"PASSPORT\", \"NATIONAL_ID\", \"DRIVING_LICENSE\", \"TAX_ID\", \"COMPANY_REGISTRATION\"]\n        },\n        \"documentNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Document number or identifier\"\n        },\n        \"issuingCountry\": {\n   \
  \       \"type\": \"string\",\n          \"description\": \"Country that issued the document\",\n          \"pattern\": \"^[A-Z]{2}$\"\n        },\n        \"issueDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Date the document was issued\"\n        },\n        \"expiryDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Document expiry date\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/json-schema/temenos-customer-schema.json
tags:
- Banking
- Cloud Banking
- Core Banking
- Digital Banking
- Financial Services
- Fintech
- Open Banking
- Payments
- Wealth Management
title: Temenos Customer
---
