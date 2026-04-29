---
description: Atm Search Request Info
layout: schema
name: AtmSearch
properties_list:
- description: Line 1 of the street address for the ATM location. Usually includes the street number and name. This parameter is ignored if latitude and longitude are provided. If you provide this parameter you must
  name: addressLine1
  type: string
- description: Line 2 of the street address usually an apartment number or suite number. This parameter is used rarely and is ignored if latitude and longitude are provided. If you provide this parameter you must al
  name: addressLine2
  type: string
- description: The name of the city for a ATM location. This parameter is ignored if latitude and longitude are provided. If you provide this parameter you must also provide the Country parameter.
  name: city
  type: string
- description: 'Any three character country code for an ATM location. Valid values are three digit alpha country codes. This parameter is ignored if latitude and longitude are provided. This parameter is required if '
  name: countryCode
  type: string
- description: The state or province for an ATM location (only supported for US and Canada locations). This parameter is ignored if latitude and longitude are provided. If you provide this parameter you must also pr
  name: countrySubdivisionCode
  type: string
- description: The latitude of a ATM location. If latitude is provided longitude must also be provided.
  name: latitude
  type: string
- description: The longitude of a ATM location. If longitude is provided latitude must also be provided.
  name: longitude
  type: string
- description: The zip code or postal code for an ATM location. This parameter is ignored if latitude and longitude are provided. If you provide this parameter you must also provide the Country parameter.
  name: postalCode
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-atm-locations-atm-search-schema.json
slug: mastercard-atm-locations-atm-search
source_filename: mastercard-atm-locations-atm-search-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AtmSearch\",\n  \"type\": \"object\",\n  \"description\": \"Atm Search Request Info\",\n  \"properties\": {\n    \"addressLine1\": {\n      \"type\": \"string\",\n      \"description\": \"Line 1 of the street address for the ATM location. Usually includes the street number and name. This parameter is ignored if latitude and longitude are provided. If you provide this parameter you must also provide the Country parameter and either City parameter or PostalCode parameter.\"\n    },\n    \"addressLine2\": {\n      \"type\": \"string\",\n      \"description\": \"Line 2 of the street address usually an apartment number or suite number. This parameter is used rarely and is ignored if latitude and longitude are provided. If you provide this parameter you must also provide the Country parameter and either City parameter or PostalCode parameter.\"\n    },\n    \"city\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The name of the city for a ATM location. This parameter is ignored if latitude and longitude are provided. If you provide this parameter you must also provide the Country parameter.\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Any three character country code for an ATM location. Valid values are three digit alpha country codes. This parameter is ignored if latitude and longitude are provided. This parameter is required if any other address information is provided including AddressLine1 AddressLine2 City PostalCode or CountrySubdivision.\"\n    },\n    \"countrySubdivisionCode\": {\n      \"type\": \"string\",\n      \"description\": \"The state or province for an ATM location (only supported for US and Canada locations). This parameter is ignored if latitude and longitude are provided. If you provide this parameter you must also provide the Country parameter.\"\n    },\n    \"latitude\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The latitude of a ATM location. If latitude is provided longitude must also be provided.\"\n    },\n    \"longitude\": {\n      \"type\": \"string\",\n      \"description\": \"The longitude of a ATM location. If longitude is provided latitude must also be provided.\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"The zip code or postal code for an ATM location. This parameter is ignored if latitude and longitude are provided. If you provide this parameter you must also provide the Country parameter.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-atm-locations-atm-search-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: AtmSearch
---
