---
description: Merchant Search Request Info
layout: schema
name: MerchantSearch
properties_list:
- description: Line 1 of the street address for the merchant location. Usually includes the street number and name. This parameter is ignored if latitude and longitude are provided. If you provide this parameter you
  name: addressLine1
  type: string
- description: Line 2 of the street address usually an apartment number or suite number. This parameter is used rarely and is ignored if latitude and longitude are provided. If you provide this parameter you must al
  name: addressLine2
  type: string
- description: The name of the city for a merchant location. This parameter is ignored if latitude and longitude are provided. If you provide this parameter you must also provide the Country parameter.
  name: city
  type: string
- description: Any two digit country code for a Merchant location. Valid values are two digit alpha country code. This parameter is ignored if latitude and longitude are provided. This parameter is required if any o
  name: countryCode
  type: string
- description: The state or province for a merchant location (only supported for US and Canada locations). This parameter is ignored if latitude and longitude are provided. If you provide this parameter you must als
  name: countrySubdivisionCode
  type: string
- description: The latitude of a merchant location. If latitude is provided longitude must also be provided.
  name: latitude
  type: string
- description: The longitude of a merchant location. If longitude is provided latitude must also be provided.
  name: longitude
  type: string
- description: Category Id of the merchant location. See the Categories resource for a list of valid categories. Input may be a comma delimited list of category ids.
  name: merchantCategory
  type: string
- description: Type of merchant location. Options are 'paypass' 'repower' 'easysavings' and 'cashback'.
  name: merchantType
  type: string
- description: Unique identifier that represents the merchant sponsor of an offer. Any valid merchant ID.
  name: offerMerchantId
  type: string
- description: The zip code or postal code for a Merchant location. This parameter is ignored if latitude and longitude are provided. If you provide this parameter you must also provide the Country parameter.
  name: postalCode
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-merchant-locations-merchant-search-schema.json
slug: mastercard-merchant-locations-merchant-search
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MerchantSearch\",\n  \"type\": \"object\",\n  \"description\": \"Merchant Search Request Info\",\n  \"properties\": {\n    \"addressLine1\": {\n      \"type\": \"string\",\n      \"description\": \"Line 1 of the street address for the merchant location. Usually includes the street number and name. This parameter is ignored if latitude and longitude are provided. If you provide this parameter you must also provide the Country parameter and either City parameter or PostalCode parameter.\"\n    },\n    \"addressLine2\": {\n      \"type\": \"string\",\n      \"description\": \"Line 2 of the street address usually an apartment number or suite number. This parameter is used rarely and is ignored if latitude and longitude are provided. If you provide this parameter you must also provide the Country parameter and either City parameter or PostalCode parameter.\"\n    },\n    \"city\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The name of the city for a merchant location. This parameter is ignored if latitude and longitude are provided. If you provide this parameter you must also provide the Country parameter.\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Any two digit country code for a Merchant location. Valid values are two digit alpha country code. This parameter is ignored if latitude and longitude are provided. This parameter is required if any other address information is provided including AddressLine1 AddressLine2 City PostalCode or CountrySubdivision.\"\n    },\n    \"countrySubdivisionCode\": {\n      \"type\": \"string\",\n      \"description\": \"The state or province for a merchant location (only supported for US and Canada locations). This parameter is ignored if latitude and longitude are provided. If you provide this parameter you must also provide the Country parameter.\"\n    },\n    \"latitude\": {\n      \"\
  type\": \"string\",\n      \"description\": \"The latitude of a merchant location. If latitude is provided longitude must also be provided.\"\n    },\n    \"longitude\": {\n      \"type\": \"string\",\n      \"description\": \"The longitude of a merchant location. If longitude is provided latitude must also be provided.\"\n    },\n    \"merchantCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Category Id of the merchant location. See the Categories resource for a list of valid categories.  Input may be a comma delimited list of category ids.\"\n    },\n    \"merchantType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of merchant location. Options are 'paypass' 'repower' 'easysavings' and 'cashback'.\"\n    },\n    \"offerMerchantId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier that represents the merchant sponsor of an offer. Any valid merchant ID.\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n     \
  \ \"description\": \"The zip code or postal code for a Merchant location. This parameter is ignored if latitude and longitude are provided. If you provide this parameter you must also provide the Country parameter.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-merchant-locations-merchant-search-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: MerchantSearch
---
