---
description: ''
layout: schema
name: BusinessPartner
properties_list:
- description: Unique identifier for the business partner
  name: CardCode
  type: string
- description: Name of the business partner
  name: CardName
  type: string
- description: Type of business partner
  name: CardType
  type: string
- description: Business partner group code
  name: GroupCode
  type: integer
- description: Primary phone number
  name: Phone1
  type: string
- description: Email address
  name: EmailAddress
  type: string
- description: Tax identification number
  name: FederalTaxID
  type: string
- description: Default currency code
  name: Currency
  type: string
- description: Whether the business partner is active
  name: Valid
  type: string
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-business-one-service-layer-business-partner-schema.json
slug: sap-business-one-service-layer-business-partner
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BusinessPartner\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CardCode\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the business partner\"\n    },\n    \"CardName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the business partner\"\n    },\n    \"CardType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of business partner\"\n    },\n    \"GroupCode\": {\n      \"type\": \"integer\",\n      \"description\": \"Business partner group code\"\n    },\n    \"Phone1\": {\n      \"type\": \"string\",\n      \"description\": \"Primary phone number\"\n    },\n    \"EmailAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Email address\"\n    },\n    \"FederalTaxID\": {\n      \"type\": \"string\",\n      \"description\": \"Tax identification number\"\n    },\n    \"Currency\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Default currency code\"\n    },\n    \"Valid\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the business partner is active\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-business-one-service-layer-business-partner-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: BusinessPartner
---
