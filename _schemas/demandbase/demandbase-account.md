---
description: Represents a company account in Demandbase with firmographic data, corporate hierarchy, and classification attributes used across ABM workflows.
layout: schema
name: Demandbase Account
properties_list:
- description: Unique Demandbase account identifier
  name: account_id
  type: string
- description: Official company name
  name: company_name
  type: string
- description: Primary web domain
  name: domain
  type: string
- description: Company website URL
  name: website
  type: string
- description: Industry classification
  name: industry
  type: string
- description: Sub-industry classification
  name: sub_industry
  type: string
- description: Standard Industrial Classification code
  name: sic_code
  type: string
- description: North American Industry Classification System code
  name: naics_code
  type: string
- description: Number of employees
  name: employee_count
  type: integer
- description: Employee count range bucket
  name: employee_range
  type: string
- description: Annual revenue in USD
  name: revenue
  type: number
- description: Revenue range bucket
  name: revenue_range
  type: string
- description: Street address
  name: address
  type: string
- description: City
  name: city
  type: string
- description: State or province
  name: state
  type: string
- description: Country
  name: country
  type: string
- description: Postal code
  name: zip
  type: string
- description: ISO country code
  name: country_code
  type: string
- description: Primary phone number
  name: phone
  type: string
- description: Stock ticker symbol
  name: stock_ticker
  type: string
- description: Year the company was founded
  name: founded_year
  type: integer
- description: Whether the company is in the Fortune 1000
  name: fortune_1000
  type: boolean
- description: Whether the company is in the Forbes 2000
  name: forbes_2000
  type: boolean
- description: Whether the company operates in the B2B space
  name: b2b
  type: boolean
- description: Whether the company operates in the B2C space
  name: b2c
  type: boolean
- description: Demandbase ID of the parent company
  name: parent_company_id
  type: string
- description: Name of the parent company
  name: parent_company_name
  type: string
- description: Demandbase ID of the ultimate parent company
  name: ultimate_parent_company_id
  type: string
- description: Name of the ultimate parent company
  name: ultimate_parent_company_name
  type: string
provider_name: Demandbase
provider_slug: demandbase
schema_file: json-schema/demandbase-account-schema.json
slug: demandbase-account
source_filename: demandbase-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.demandbase.com/schemas/demandbase/account.json\",\n  \"title\": \"Demandbase Account\",\n  \"description\": \"Represents a company account in Demandbase with firmographic data, corporate hierarchy, and classification attributes used across ABM workflows.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"account_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Demandbase account identifier\"\n    },\n    \"company_name\": {\n      \"type\": \"string\",\n      \"description\": \"Official company name\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Primary web domain\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Company website URL\"\n    },\n    \"industry\": {\n      \"type\": \"string\",\n      \"description\": \"Industry classification\"\n    },\n    \"\
  sub_industry\": {\n      \"type\": \"string\",\n      \"description\": \"Sub-industry classification\"\n    },\n    \"sic_code\": {\n      \"type\": \"string\",\n      \"description\": \"Standard Industrial Classification code\"\n    },\n    \"naics_code\": {\n      \"type\": \"string\",\n      \"description\": \"North American Industry Classification System code\"\n    },\n    \"employee_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of employees\"\n    },\n    \"employee_range\": {\n      \"type\": \"string\",\n      \"description\": \"Employee count range bucket\"\n    },\n    \"revenue\": {\n      \"type\": \"number\",\n      \"description\": \"Annual revenue in USD\"\n    },\n    \"revenue_range\": {\n      \"type\": \"string\",\n      \"description\": \"Revenue range bucket\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Street address\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"\
  City\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State or province\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country\"\n    },\n    \"zip\": {\n      \"type\": \"string\",\n      \"description\": \"Postal code\"\n    },\n    \"country_code\": {\n      \"type\": \"string\",\n      \"description\": \"ISO country code\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Primary phone number\"\n    },\n    \"stock_ticker\": {\n      \"type\": \"string\",\n      \"description\": \"Stock ticker symbol\"\n    },\n    \"founded_year\": {\n      \"type\": \"integer\",\n      \"description\": \"Year the company was founded\"\n    },\n    \"fortune_1000\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the company is in the Fortune 1000\"\n    },\n    \"forbes_2000\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the company is in the Forbes 2000\"\
  \n    },\n    \"b2b\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the company operates in the B2B space\"\n    },\n    \"b2c\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the company operates in the B2C space\"\n    },\n    \"parent_company_id\": {\n      \"type\": \"string\",\n      \"description\": \"Demandbase ID of the parent company\"\n    },\n    \"parent_company_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the parent company\"\n    },\n    \"ultimate_parent_company_id\": {\n      \"type\": \"string\",\n      \"description\": \"Demandbase ID of the ultimate parent company\"\n    },\n    \"ultimate_parent_company_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the ultimate parent company\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/json-schema/demandbase-account-schema.json
tags:
- Account-Based Marketing
- Advertising
- AI Agents
- B2B Marketing
- Data Enrichment
- Intent Data
- Personalization
- Sales Intelligence
title: Demandbase Account
---
