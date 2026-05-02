---
description: A Marqeta cardholder (user) record representing an individual who holds one or more payment cards on the Marqeta platform. Cardholders can have funds loaded onto their general purpose account (GPA), be subject to KYC verification, and be organized into account holder groups for applying shared spending controls.
layout: schema
name: Marqeta Cardholder
properties_list:
- description: Unique identifier for the cardholder on the Marqeta platform.
  name: token
  type: string
- description: Cardholder's first name.
  name: first_name
  type: string
- description: Cardholder's middle name.
  name: middle_name
  type: string
- description: Cardholder's last name.
  name: last_name
  type: string
- description: Cardholder's email address.
  name: email
  type: string
- description: Cardholder's phone number in E.164 format.
  name: phone
  type: string
- description: Current account status of the cardholder.
  name: status
  type: string
- description: KYC verification requirement level for this cardholder.
  name: kyc_required
  type: string
- description: Primary street address line.
  name: address1
  type: string
- description: Secondary address line (apartment, suite, unit).
  name: address2
  type: string
- description: City of residence.
  name: city
  type: string
- description: State or province of residence (two-letter abbreviation for US states).
  name: state
  type: string
- description: ZIP or postal code.
  name: zip
  type: string
- description: Two-letter ISO 3166-1 alpha-2 country code.
  name: country
  type: string
- description: Cardholder's date of birth (YYYY-MM-DD).
  name: birth_date
  type: string
- description: Social Security Number (last 4 or full 9 digits). Used for KYC identity verification.
  name: ssn
  type: string
- description: Passport number for non-US identity verification.
  name: passport_number
  type: string
- description: Passport expiration date (YYYY-MM-DD).
  name: passport_expiration_date
  type: string
- description: Cardholder's nationality (two-letter ISO country code).
  name: nationality
  type: string
- description: If true, this cardholder is designated as a corporate card holder.
  name: corporate_card_holder
  type: boolean
- description: Token of the account holder group this cardholder belongs to.
  name: account_holder_group_token
  type: string
- description: ''
  name: authentication
  type: object
- description: List of government-issued identity documents associated with this cardholder.
  name: identifications
  type: array
- description: Key-value pairs of custom metadata associated with this cardholder. Maximum 20 pairs, values must be strings.
  name: metadata
  type: object
- description: ISO 8601 timestamp when the cardholder was created.
  name: created_time
  type: string
- description: ISO 8601 timestamp when the cardholder record was last modified.
  name: last_modified_time
  type: string
provider_name: marqeta
provider_slug: marqeta
schema_file: json-schema/marqeta-cardholder-schema.json
slug: marqeta-cardholder
source_filename: marqeta-cardholder-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://marqeta.com/schemas/cardholder.json\",\n  \"title\": \"Marqeta Cardholder\",\n  \"description\": \"A Marqeta cardholder (user) record representing an individual who holds one or more payment cards on the Marqeta platform. Cardholders can have funds loaded onto their general purpose account (GPA), be subject to KYC verification, and be organized into account holder groups for applying shared spending controls.\",\n  \"type\": \"object\",\n  \"required\": [\"token\", \"status\", \"created_time\"],\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the cardholder on the Marqeta platform.\",\n      \"maxLength\": 36\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"Cardholder's first name.\",\n      \"maxLength\": 40\n    },\n    \"middle_name\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Cardholder's middle name.\",\n      \"maxLength\": 40\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Cardholder's last name.\",\n      \"maxLength\": 40\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Cardholder's email address.\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Cardholder's phone number in E.164 format.\",\n      \"pattern\": \"^\\\\+?[1-9]\\\\d{1,14}$\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current account status of the cardholder.\",\n      \"enum\": [\"ACTIVE\", \"SUSPENDED\", \"CLOSED\", \"UNVERIFIED\", \"LIMITED\"]\n    },\n    \"kyc_required\": {\n      \"type\": \"string\",\n      \"description\": \"KYC verification requirement level for this cardholder.\",\n      \"enum\": [\"NOT_REQUIRED\", \"CONDITIONAL\", \"ALWAYS\"]\n    },\n    \"address1\": {\n      \"type\": \"string\",\n   \
  \   \"description\": \"Primary street address line.\",\n      \"maxLength\": 255\n    },\n    \"address2\": {\n      \"type\": \"string\",\n      \"description\": \"Secondary address line (apartment, suite, unit).\",\n      \"maxLength\": 255\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City of residence.\",\n      \"maxLength\": 40\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State or province of residence (two-letter abbreviation for US states).\",\n      \"maxLength\": 32\n    },\n    \"zip\": {\n      \"type\": \"string\",\n      \"description\": \"ZIP or postal code.\",\n      \"maxLength\": 10\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Two-letter ISO 3166-1 alpha-2 country code.\",\n      \"pattern\": \"^[A-Z]{2}$\"\n    },\n    \"birth_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Cardholder's date of birth (YYYY-MM-DD).\"\
  \n    },\n    \"ssn\": {\n      \"type\": \"string\",\n      \"description\": \"Social Security Number (last 4 or full 9 digits). Used for KYC identity verification.\",\n      \"pattern\": \"^(\\\\d{4}|\\\\d{9})$\"\n    },\n    \"passport_number\": {\n      \"type\": \"string\",\n      \"description\": \"Passport number for non-US identity verification.\",\n      \"maxLength\": 40\n    },\n    \"passport_expiration_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Passport expiration date (YYYY-MM-DD).\"\n    },\n    \"nationality\": {\n      \"type\": \"string\",\n      \"description\": \"Cardholder's nationality (two-letter ISO country code).\",\n      \"pattern\": \"^[A-Z]{2}$\"\n    },\n    \"corporate_card_holder\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, this cardholder is designated as a corporate card holder.\"\n    },\n    \"account_holder_group_token\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Token of the account holder group this cardholder belongs to.\",\n      \"maxLength\": 36\n    },\n    \"authentication\": {\n      \"$ref\": \"#/$defs/CardholderAuthentication\"\n    },\n    \"identifications\": {\n      \"type\": \"array\",\n      \"description\": \"List of government-issued identity documents associated with this cardholder.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Identification\"\n      }\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value pairs of custom metadata associated with this cardholder. Maximum 20 pairs, values must be strings.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"maxProperties\": 20\n    },\n    \"created_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the cardholder was created.\"\n    },\n    \"last_modified_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"ISO 8601 timestamp when the cardholder record was last modified.\"\n    }\n  },\n  \"$defs\": {\n    \"CardholderAuthentication\": {\n      \"type\": \"object\",\n      \"description\": \"Authentication configuration for this cardholder.\",\n      \"properties\": {\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Email address used for authentication notifications.\"\n        },\n        \"last_four_digits\": {\n          \"type\": \"string\",\n          \"description\": \"Last four digits of the card used for authentication.\",\n          \"pattern\": \"^\\\\d{4}$\"\n        }\n      }\n    },\n    \"Identification\": {\n      \"type\": \"object\",\n      \"description\": \"Government-issued identification document for KYC purposes.\",\n      \"required\": [\"type\", \"value\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Type\
  \ of identification document.\",\n          \"enum\": [\"SSN\", \"PASSPORT\", \"DRIVERS_LICENSE\", \"SIN\", \"NIN\"]\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"Identification document number or value.\",\n          \"maxLength\": 255\n        },\n        \"expiration_date\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Expiration date of the document (YYYY-MM-DD).\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/marqeta/refs/heads/main/json-schema/marqeta-cardholder-schema.json
tags: []
title: Marqeta Cardholder
---
