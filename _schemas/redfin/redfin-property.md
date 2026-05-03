---
description: A real estate property listing as represented in the Redfin Stingray API, including address, price, physical characteristics, and listing metadata.
layout: schema
name: Redfin Property
properties_list:
- description: Unique Redfin property identifier.
  name: propertyId
  type: integer
- description: Unique Redfin listing identifier. A property may have multiple listings over time.
  name: listingId
  type: integer
- description: MLS listing identifier assigned by the local Multiple Listing Service.
  name: mlsId
  type: string
- description: ''
  name: address
  type: object
- description: Current listing or last sale price in USD.
  name: price
  type: number
- description: Number of bedrooms.
  name: beds
  type: integer
- description: Number of bathrooms, may include half-baths as 0.5.
  name: baths
  type: number
- description: Approximate living area in square feet.
  name: sqFt
  type: integer
- description: Lot size in square feet.
  name: lotSize
  type: integer
- description: Year the property was constructed.
  name: yearBuilt
  type: integer
- description: Number of stories or levels in the building.
  name: stories
  type: integer
- description: Type of property.
  name: propertyType
  type: string
- description: Numeric property type code (1=house, 2=condo, 3=townhouse, 4=multi-family, 5=land, 6=other).
  name: propertyTypeCode
  type: integer
- description: Current listing status.
  name: listingStatus
  type: string
- description: Type of listing source (e.g., MLS, FSBO).
  name: listingType
  type: string
- description: Number of days the property has been actively listed.
  name: daysOnMarket
  type: integer
- description: Latitude coordinate of the property.
  name: latitude
  type: number
- description: Longitude coordinate of the property.
  name: longitude
  type: number
- description: Relative URL path to the property listing on Redfin.
  name: url
  type: string
- description: Redfin automated valuation model (AVM) estimate in USD.
  name: redfinEstimate
  type: number
- description: Whether the property has a garage.
  name: hasGarage
  type: boolean
- description: Whether the property has a basement.
  name: hasBasement
  type: boolean
- description: Number of parking spaces.
  name: parkingSpaces
  type: integer
- description: Monthly HOA fee in USD, 0 if no HOA.
  name: hoaFee
  type: number
- description: Historical events for the property including sales, price changes, and listing status changes.
  name: history
  type: array
provider_name: Redfin
provider_slug: redfin
schema_file: json-schema/redfin-property-schema.json
slug: redfin-property
source_filename: redfin-property-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://redfin.com/schemas/redfin/property.json\",\n  \"title\": \"Redfin Property\",\n  \"description\": \"A real estate property listing as represented in the Redfin Stingray API, including address, price, physical characteristics, and listing metadata.\",\n  \"type\": \"object\",\n  \"required\": [\"propertyId\", \"address\"],\n  \"properties\": {\n    \"propertyId\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique Redfin property identifier.\"\n    },\n    \"listingId\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique Redfin listing identifier. A property may have multiple listings over time.\"\n    },\n    \"mlsId\": {\n      \"type\": \"string\",\n      \"description\": \"MLS listing identifier assigned by the local Multiple Listing Service.\"\n    },\n    \"address\": {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"price\": {\n      \"type\": \"number\"\
  ,\n      \"minimum\": 0,\n      \"description\": \"Current listing or last sale price in USD.\"\n    },\n    \"beds\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of bedrooms.\"\n    },\n    \"baths\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Number of bathrooms, may include half-baths as 0.5.\"\n    },\n    \"sqFt\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Approximate living area in square feet.\"\n    },\n    \"lotSize\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Lot size in square feet.\"\n    },\n    \"yearBuilt\": {\n      \"type\": \"integer\",\n      \"minimum\": 1600,\n      \"maximum\": 2030,\n      \"description\": \"Year the property was constructed.\"\n    },\n    \"stories\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"Number of stories or levels in the building.\"\n    },\n \
  \   \"propertyType\": {\n      \"type\": \"string\",\n      \"enum\": [\"house\", \"condo\", \"townhouse\", \"multi-family\", \"land\", \"other\"],\n      \"description\": \"Type of property.\"\n    },\n    \"propertyTypeCode\": {\n      \"type\": \"integer\",\n      \"enum\": [1, 2, 3, 4, 5, 6],\n      \"description\": \"Numeric property type code (1=house, 2=condo, 3=townhouse, 4=multi-family, 5=land, 6=other).\"\n    },\n    \"listingStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"pending\", \"sold\", \"off-market\", \"contingent\"],\n      \"description\": \"Current listing status.\"\n    },\n    \"listingType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of listing source (e.g., MLS, FSBO).\"\n    },\n    \"daysOnMarket\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of days the property has been actively listed.\"\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"minimum\": -90,\n\
  \      \"maximum\": 90,\n      \"description\": \"Latitude coordinate of the property.\"\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"minimum\": -180,\n      \"maximum\": 180,\n      \"description\": \"Longitude coordinate of the property.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Relative URL path to the property listing on Redfin.\"\n    },\n    \"redfinEstimate\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Redfin automated valuation model (AVM) estimate in USD.\"\n    },\n    \"hasGarage\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the property has a garage.\"\n    },\n    \"hasBasement\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the property has a basement.\"\n    },\n    \"parkingSpaces\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of parking spaces.\"\n    },\n    \"hoaFee\": {\n      \"type\"\
  : \"number\",\n      \"minimum\": 0,\n      \"description\": \"Monthly HOA fee in USD, 0 if no HOA.\"\n    },\n    \"history\": {\n      \"type\": \"array\",\n      \"description\": \"Historical events for the property including sales, price changes, and listing status changes.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PropertyHistoryEvent\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"Physical address of a property.\",\n      \"required\": [\"streetAddress\", \"city\", \"state\", \"zip\"],\n      \"properties\": {\n        \"streetAddress\": {\n          \"type\": \"string\",\n          \"description\": \"Street number and name.\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"City name.\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"minLength\": 2,\n          \"maxLength\": 2,\n          \"pattern\": \"^[A-Z]{2}$\",\n      \
  \    \"description\": \"Two-letter US state abbreviation.\"\n        },\n        \"zip\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[0-9]{5}(-[0-9]{4})?$\",\n          \"description\": \"5-digit or 9-digit US ZIP code.\"\n        }\n      }\n    },\n    \"PropertyHistoryEvent\": {\n      \"type\": \"object\",\n      \"description\": \"A historical event in a property's listing or sale history.\",\n      \"required\": [\"eventDate\", \"eventType\"],\n      \"properties\": {\n        \"eventDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Date of the event.\"\n        },\n        \"eventType\": {\n          \"type\": \"string\",\n          \"enum\": [\"Listed\", \"Sold\", \"PriceChange\", \"Pending\", \"Delisted\", \"Relisted\"],\n          \"description\": \"Type of historical event.\"\n        },\n        \"price\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"description\": \"Price\
  \ associated with the event in USD.\"\n        },\n        \"source\": {\n          \"type\": \"string\",\n          \"description\": \"Data source for the event record (e.g., MLS name).\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/redfin/refs/heads/main/json-schema/redfin-property-schema.json
tags:
- CSV Export
- GIS
- Home Values
- Housing Market
- Listings
- Property Data
- Real Estate
title: Redfin Property
---
