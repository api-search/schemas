---
description: ''
layout: schema
name: BusinessPartnerAddress
properties_list:
- description: Business partner number
  name: BusinessPartner
  type: string
- description: Address identifier
  name: AddressID
  type: string
- description: Country key (ISO 3166-1 alpha-2)
  name: Country
  type: string
- description: Region or state code
  name: Region
  type: string
- description: City name
  name: CityName
  type: string
- description: Postal code
  name: PostalCode
  type: string
- description: Street name
  name: StreetName
  type: string
- description: House number
  name: HouseNumber
  type: string
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-s4hana-cloud-business-partner-business-partner-address-schema.json
slug: sap-s4hana-cloud-business-partner-business-partner-address
source_filename: sap-s4hana-cloud-business-partner-business-partner-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BusinessPartnerAddress\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BusinessPartner\": {\n      \"type\": \"string\",\n      \"description\": \"Business partner number\"\n    },\n    \"AddressID\": {\n      \"type\": \"string\",\n      \"description\": \"Address identifier\"\n    },\n    \"Country\": {\n      \"type\": \"string\",\n      \"description\": \"Country key (ISO 3166-1 alpha-2)\"\n    },\n    \"Region\": {\n      \"type\": \"string\",\n      \"description\": \"Region or state code\"\n    },\n    \"CityName\": {\n      \"type\": \"string\",\n      \"description\": \"City name\"\n    },\n    \"PostalCode\": {\n      \"type\": \"string\",\n      \"description\": \"Postal code\"\n    },\n    \"StreetName\": {\n      \"type\": \"string\",\n      \"description\": \"Street name\"\n    },\n    \"HouseNumber\": {\n      \"type\": \"string\",\n      \"description\": \"House number\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-s4hana-cloud-business-partner-business-partner-address-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: BusinessPartnerAddress
---
