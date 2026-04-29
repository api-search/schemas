---
description: Company entity metadata and recent filing history from the SEC EDGAR Submissions API.
layout: schema
name: EdgarCompanySubmission
properties_list:
- description: Central Index Key — unique 10-digit identifier assigned by the SEC
  name: cik
  type: string
- description: Type of entity registered with the SEC
  name: entityType
  type: string
- description: Standard Industrial Classification code
  name: sic
  type: string
- description: Description of the SIC code industry
  name: sicDescription
  type: string
- description: Current legal name of the entity
  name: name
  type: string
- description: Stock ticker symbols for the entity
  name: tickers
  type: array
- description: Stock exchanges where the entity is listed
  name: exchanges
  type: array
- description: US state code or country of incorporation
  name: stateOfIncorporation
  type: string
- description: Month and day of fiscal year end (MMDD)
  name: fiscalYearEnd
  type: string
- description: Official website of the entity
  name: website
  type: string
- description: Recent filing history
  name: filings
  type: object
provider_name: Accounting Standards
provider_slug: accounting-standards
schema_file: json-schema/edgar-company-submission-schema.json
slug: edgar-company-submission
source_filename: edgar-company-submission-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accounting-standards/refs/heads/main/json-schema/edgar-company-submission-schema.json\",\n  \"title\": \"EdgarCompanySubmission\",\n  \"description\": \"Company entity metadata and recent filing history from the SEC EDGAR Submissions API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cik\": {\n      \"type\": \"string\",\n      \"description\": \"Central Index Key — unique 10-digit identifier assigned by the SEC\",\n      \"example\": \"0000320193\"\n    },\n    \"entityType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of entity registered with the SEC\",\n      \"example\": \"operating\"\n    },\n    \"sic\": {\n      \"type\": \"string\",\n      \"description\": \"Standard Industrial Classification code\",\n      \"example\": \"3674\"\n    },\n    \"sicDescription\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Description of the SIC code industry\",\n      \"example\": \"Semiconductors And Related Devices\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Current legal name of the entity\",\n      \"example\": \"Apple Inc.\"\n    },\n    \"tickers\": {\n      \"type\": \"array\",\n      \"description\": \"Stock ticker symbols for the entity\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\"AAPL\"]\n    },\n    \"exchanges\": {\n      \"type\": \"array\",\n      \"description\": \"Stock exchanges where the entity is listed\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\"Nasdaq\"]\n    },\n    \"stateOfIncorporation\": {\n      \"type\": \"string\",\n      \"description\": \"US state code or country of incorporation\",\n      \"example\": \"CA\"\n    },\n    \"fiscalYearEnd\": {\n      \"type\": \"string\",\n      \"description\": \"Month and day of fiscal year end (MMDD)\",\n      \"example\"\
  : \"0928\",\n      \"pattern\": \"^[0-9]{4}$\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Official website of the entity\",\n      \"example\": \"https://www.apple.com\"\n    },\n    \"filings\": {\n      \"type\": \"object\",\n      \"description\": \"Recent filing history\",\n      \"properties\": {\n        \"recent\": {\n          \"type\": \"object\",\n          \"description\": \"Most recent filings metadata arrays\",\n          \"properties\": {\n            \"accessionNumber\": {\n              \"type\": \"array\",\n              \"items\": {\"type\": \"string\"},\n              \"example\": [\"0000320193-25-000001\"]\n            },\n            \"filingDate\": {\n              \"type\": \"array\",\n              \"items\": {\"type\": \"string\", \"format\": \"date\"},\n              \"example\": [\"2025-02-01\"]\n            },\n            \"form\": {\n              \"type\": \"array\",\n              \"items\"\
  : {\"type\": \"string\"},\n              \"example\": [\"10-K\"]\n            },\n            \"primaryDocument\": {\n              \"type\": \"array\",\n              \"items\": {\"type\": \"string\"},\n              \"example\": [\"aapl-20240928.htm\"]\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"cik\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accounting-standards/refs/heads/main/json-schema/edgar-company-submission-schema.json
tags:
- Accounting Standards
- Finance
- GAAP
- IFRS
- XBRL
- Financial Reporting
- SEC
- FASB
title: EdgarCompanySubmission
---
