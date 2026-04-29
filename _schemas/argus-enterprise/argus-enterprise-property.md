---
description: Represents a commercial real estate property in the ARGUS Enterprise platform, including physical attributes, financial metrics, and portfolio association.
layout: schema
name: Argus Enterprise Property
properties_list:
- description: Unique property identifier
  name: id
  type: string
- description: Property name
  name: name
  type: string
- description: Type of commercial real estate property
  name: propertyType
  type: string
- description: Current property status
  name: status
  type: string
- description: Property physical address
  name: address
  type: object
- description: Gross leasable area in square feet
  name: grossArea
  type: number
- description: Net leasable area in square feet
  name: netLeasableArea
  type: number
- description: Year the property was built
  name: yearBuilt
  type: integer
- description: Number of leasable units or suites
  name: numberOfUnits
  type: integer
- description: Original purchase price
  name: purchasePrice
  type: number
- description: Date of property acquisition
  name: purchaseDate
  type: string
- description: Current estimated market value
  name: currentMarketValue
  type: number
- description: Current occupancy rate as a percentage
  name: occupancyRate
  type: number
- description: Identifier of the parent portfolio
  name: portfolioId
  type: string
- description: Record creation timestamp
  name: createdAt
  type: string
- description: Record last update timestamp
  name: updatedAt
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-property-schema.json
slug: argus-enterprise-property
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.argusenterprise.com/schemas/argus-enterprise/property.json\",\n  \"title\": \"Argus Enterprise Property\",\n  \"description\": \"Represents a commercial real estate property in the ARGUS Enterprise platform, including physical attributes, financial metrics, and portfolio association.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique property identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Property name\"\n    },\n    \"propertyType\": {\n      \"type\": \"string\",\n      \"enum\": [\"Office\", \"Retail\", \"Industrial\", \"Multifamily\", \"Mixed-Use\", \"Hotel\", \"Land\", \"Other\"],\n      \"description\": \"Type of commercial real estate property\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Active\"\
  , \"Pending\", \"Archived\"],\n      \"description\": \"Current property status\"\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"description\": \"Property physical address\",\n      \"properties\": {\n        \"street\": {\n          \"type\": \"string\",\n          \"description\": \"Street address\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"City\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"State or province\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\",\n          \"description\": \"Postal or ZIP code\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"Country code (ISO 3166-1 alpha-2)\"\n        }\n      }\n    },\n    \"grossArea\": {\n      \"type\": \"number\",\n      \"description\": \"Gross leasable area in square feet\"\n    },\n    \"netLeasableArea\": {\n      \"type\": \"number\"\
  ,\n      \"description\": \"Net leasable area in square feet\"\n    },\n    \"yearBuilt\": {\n      \"type\": \"integer\",\n      \"description\": \"Year the property was built\"\n    },\n    \"numberOfUnits\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of leasable units or suites\"\n    },\n    \"purchasePrice\": {\n      \"type\": \"number\",\n      \"description\": \"Original purchase price\"\n    },\n    \"purchaseDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of property acquisition\"\n    },\n    \"currentMarketValue\": {\n      \"type\": \"number\",\n      \"description\": \"Current estimated market value\"\n    },\n    \"occupancyRate\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Current occupancy rate as a percentage\"\n    },\n    \"portfolioId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Identifier\
  \ of the parent portfolio\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record creation timestamp\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record last update timestamp\"\n    }\n  },\n  \"required\": [\"name\", \"propertyType\", \"address\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-property-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: Argus Enterprise Property
---
