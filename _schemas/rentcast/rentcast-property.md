---
description: A US real estate property record from the RentCast API, containing public record data for residential and commercial properties
layout: schema
name: RentCast Property Record
properties_list:
- description: Unique property identifier in the RentCast database
  name: id
  type: string
- description: Full formatted address string
  name: formattedAddress
  type: string
- description: Street address line 1
  name: addressLine1
  type: string
- description: Street address line 2 (unit, apt, etc.)
  name: addressLine2
  type: string
- description: City name
  name: city
  type: string
- description: 2-character US state abbreviation
  name: state
  type: string
- description: 5-digit ZIP code
  name: zipCode
  type: string
- description: County name
  name: county
  type: string
- description: Geographic latitude coordinate
  name: latitude
  type: number
- description: Geographic longitude coordinate
  name: longitude
  type: number
- description: Property classification
  name: propertyType
  type: string
- description: Number of bedrooms
  name: bedrooms
  type: number
- description: Number of bathrooms including partial
  name: bathrooms
  type: number
- description: Total living area in square feet
  name: squareFootage
  type: integer
- description: Lot size in square feet
  name: lotSize
  type: integer
- description: Year the property was constructed
  name: yearBuilt
  type: integer
- description: Tax-assessed value of the property in USD
  name: assessedValue
  type: number
- description: Date of the most recent sale
  name: lastSaleDate
  type: string
- description: Price of the most recent sale in USD
  name: lastSalePrice
  type: number
- description: Whether the property is owner-occupied
  name: ownerOccupied
  type: boolean
- description: Property owner information
  name: owner
  type: object
provider_name: RentCast
provider_slug: rentcast
schema_file: json-schema/rentcast-property-schema.json
slug: rentcast-property
source_filename: rentcast-property-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api.rentcast.io/schemas/property\",\n  \"title\": \"RentCast Property Record\",\n  \"description\": \"A US real estate property record from the RentCast API, containing public record data for residential and commercial properties\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"addressLine1\", \"city\", \"state\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique property identifier in the RentCast database\"\n    },\n    \"formattedAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Full formatted address string\",\n      \"example\": \"123 Main St, Austin, TX 78701\"\n    },\n    \"addressLine1\": {\n      \"type\": \"string\",\n      \"description\": \"Street address line 1\",\n      \"example\": \"123 Main St\"\n    },\n    \"addressLine2\": {\n      \"type\": \"string\",\n      \"description\": \"Street address line\
  \ 2 (unit, apt, etc.)\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City name\",\n      \"example\": \"Austin\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"2-character US state abbreviation\",\n      \"example\": \"TX\"\n    },\n    \"zipCode\": {\n      \"type\": \"string\",\n      \"description\": \"5-digit ZIP code\",\n      \"example\": \"78701\"\n    },\n    \"county\": {\n      \"type\": \"string\",\n      \"description\": \"County name\",\n      \"example\": \"Travis\"\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"description\": \"Geographic latitude coordinate\",\n      \"example\": 30.2672\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"description\": \"Geographic longitude coordinate\",\n      \"example\": -97.7431\n    },\n    \"propertyType\": {\n      \"type\": \"string\",\n      \"description\": \"Property classification\",\n      \"enum\": [\"Single Family\"\
  , \"Condo\", \"Townhouse\", \"Manufactured\", \"Multi-Family\", \"Apartment\", \"Land\"]\n    },\n    \"bedrooms\": {\n      \"type\": \"number\",\n      \"description\": \"Number of bedrooms\",\n      \"example\": 3\n    },\n    \"bathrooms\": {\n      \"type\": \"number\",\n      \"description\": \"Number of bathrooms including partial\",\n      \"example\": 2.5\n    },\n    \"squareFootage\": {\n      \"type\": \"integer\",\n      \"description\": \"Total living area in square feet\",\n      \"example\": 1800\n    },\n    \"lotSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Lot size in square feet\",\n      \"example\": 7500\n    },\n    \"yearBuilt\": {\n      \"type\": \"integer\",\n      \"description\": \"Year the property was constructed\",\n      \"example\": 1995\n    },\n    \"assessedValue\": {\n      \"type\": \"number\",\n      \"description\": \"Tax-assessed value of the property in USD\",\n      \"example\": 320000\n    },\n    \"lastSaleDate\": {\n  \
  \    \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of the most recent sale\",\n      \"example\": \"2022-06-15\"\n    },\n    \"lastSalePrice\": {\n      \"type\": \"number\",\n      \"description\": \"Price of the most recent sale in USD\",\n      \"example\": 425000\n    },\n    \"ownerOccupied\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the property is owner-occupied\"\n    },\n    \"owner\": {\n      \"type\": \"object\",\n      \"description\": \"Property owner information\",\n      \"properties\": {\n        \"names\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"Owner name(s)\"\n        },\n        \"mailingAddress\": {\n          \"type\": \"object\",\n          \"description\": \"Owner mailing address\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rentcast/refs/heads/main/json-schema/rentcast-property-schema.json
tags:
- Real Estate
- Property Data
- Valuation
- Rental Market
- AVM
title: RentCast Property Record
---
