---
description: Represents a property valuation in the ARGUS Enterprise platform, capturing DCF analysis, direct capitalization, or comparable sales methodology results including key financial metrics.
layout: schema
name: Argus Enterprise Valuation
properties_list:
- description: Unique valuation identifier
  name: id
  type: string
- description: Associated property identifier
  name: propertyId
  type: string
- description: Date of valuation
  name: valuationDate
  type: string
- description: Valuation methodology used
  name: methodology
  type: string
- description: Estimated market value
  name: marketValue
  type: number
- description: Capitalization rate (percentage)
  name: capRate
  type: number
- description: Discount rate used in DCF analysis (percentage)
  name: discountRate
  type: number
- description: Terminal capitalization rate for DCF analysis (percentage)
  name: terminalCapRate
  type: number
- description: Start date of the analysis period
  name: analysisStartDate
  type: string
- description: End date of the analysis period
  name: analysisEndDate
  type: string
- description: Stabilized net operating income
  name: netOperatingIncome
  type: number
- description: Net present value from DCF analysis
  name: netPresentValue
  type: number
- description: Internal rate of return (percentage)
  name: internalRateOfReturn
  type: number
- description: Currency code (ISO 4217)
  name: currency
  type: string
- description: Additional notes or assumptions
  name: notes
  type: string
- description: Username of the creator
  name: createdBy
  type: string
- description: Record creation timestamp
  name: createdAt
  type: string
- description: Record last update timestamp
  name: updatedAt
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-valuation-schema.json
slug: argus-enterprise-valuation
source_filename: argus-enterprise-valuation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.argusenterprise.com/schemas/argus-enterprise/valuation.json\",\n  \"title\": \"Argus Enterprise Valuation\",\n  \"description\": \"Represents a property valuation in the ARGUS Enterprise platform, capturing DCF analysis, direct capitalization, or comparable sales methodology results including key financial metrics.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique valuation identifier\"\n    },\n    \"propertyId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Associated property identifier\"\n    },\n    \"valuationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of valuation\"\n    },\n    \"methodology\": {\n      \"type\": \"string\",\n      \"enum\": [\"DCF\", \"DirectCapitalization\"\
  , \"ComparableSales\"],\n      \"description\": \"Valuation methodology used\"\n    },\n    \"marketValue\": {\n      \"type\": \"number\",\n      \"description\": \"Estimated market value\"\n    },\n    \"capRate\": {\n      \"type\": \"number\",\n      \"description\": \"Capitalization rate (percentage)\"\n    },\n    \"discountRate\": {\n      \"type\": \"number\",\n      \"description\": \"Discount rate used in DCF analysis (percentage)\"\n    },\n    \"terminalCapRate\": {\n      \"type\": \"number\",\n      \"description\": \"Terminal capitalization rate for DCF analysis (percentage)\"\n    },\n    \"analysisStartDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Start date of the analysis period\"\n    },\n    \"analysisEndDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"End date of the analysis period\"\n    },\n    \"netOperatingIncome\": {\n      \"type\": \"number\",\n      \"description\"\
  : \"Stabilized net operating income\"\n    },\n    \"netPresentValue\": {\n      \"type\": \"number\",\n      \"description\": \"Net present value from DCF analysis\"\n    },\n    \"internalRateOfReturn\": {\n      \"type\": \"number\",\n      \"description\": \"Internal rate of return (percentage)\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code (ISO 4217)\",\n      \"default\": \"USD\"\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Additional notes or assumptions\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the creator\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record creation timestamp\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record last update timestamp\"\n    }\n  },\n  \"required\": [\"valuationDate\"\
  , \"methodology\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-valuation-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: Argus Enterprise Valuation
---
