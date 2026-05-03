---
description: A registrant entity registered with the SEC in EDGAR
layout: schema
name: SEC EDGAR Company
properties_list:
- description: Central Index Key — unique 10-digit identifier with leading zeros
  name: cik
  type: string
- description: Company/registrant name as filed with SEC
  name: name
  type: string
- description: Stock exchange ticker symbols
  name: tickers
  type: array
- description: Stock exchanges where listed
  name: exchanges
  type: array
- description: Standard Industrial Classification (SIC) code
  name: sic
  type: string
- description: SIC industry description
  name: sicDescription
  type: string
- description: Employer Identification Number (XX-XXXXXXX)
  name: ein
  type: string
- description: SEC entity type classification
  name: entityType
  type: string
- description: Fiscal year end as MMDD
  name: fiscalYearEnd
  type: string
- description: US state or country code of incorporation
  name: stateOfIncorporation
  type: string
- description: ''
  name: addresses
  type: object
- description: ''
  name: website
  type: string
- description: SEC filer category
  name: category
  type: string
provider_name: sec-edgar
provider_slug: sec-edgar
schema_file: json-schema/sec-edgar-company-schema.json
slug: sec-edgar-company
source_filename: sec-edgar-company-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://data.sec.gov/schemas/company\",\n  \"title\": \"SEC EDGAR Company\",\n  \"description\": \"A registrant entity registered with the SEC in EDGAR\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cik\": {\n      \"type\": \"string\",\n      \"description\": \"Central Index Key — unique 10-digit identifier with leading zeros\",\n      \"pattern\": \"^\\\\d{10}$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Company/registrant name as filed with SEC\"\n    },\n    \"tickers\": {\n      \"type\": \"array\",\n      \"description\": \"Stock exchange ticker symbols\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"exchanges\": {\n      \"type\": \"array\",\n      \"description\": \"Stock exchanges where listed\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"NYSE\", \"Nasdaq\", \"NYSE MKT\", \"NYSE Arca\"\
  , \"OTC\", \"CBOE\"]\n      }\n    },\n    \"sic\": {\n      \"type\": \"string\",\n      \"description\": \"Standard Industrial Classification (SIC) code\",\n      \"pattern\": \"^\\\\d{4}$\"\n    },\n    \"sicDescription\": {\n      \"type\": \"string\",\n      \"description\": \"SIC industry description\"\n    },\n    \"ein\": {\n      \"type\": \"string\",\n      \"description\": \"Employer Identification Number (XX-XXXXXXX)\",\n      \"pattern\": \"^\\\\d{2}-\\\\d{7}$\"\n    },\n    \"entityType\": {\n      \"type\": \"string\",\n      \"enum\": [\"operating\", \"investment\", \"sab99\", \"special purpose\"],\n      \"description\": \"SEC entity type classification\"\n    },\n    \"fiscalYearEnd\": {\n      \"type\": \"string\",\n      \"description\": \"Fiscal year end as MMDD\",\n      \"pattern\": \"^\\\\d{4}$\",\n      \"examples\": [\"0930\", \"1231\"]\n    },\n    \"stateOfIncorporation\": {\n      \"type\": \"string\",\n      \"description\": \"US state or country code of incorporation\"\
  \n    },\n    \"addresses\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"mailing\": {\n          \"$ref\": \"#/$defs/Address\"\n        },\n        \"business\": {\n          \"$ref\": \"#/$defs/Address\"\n        }\n      }\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"SEC filer category\",\n      \"examples\": [\n        \"Large accelerated filer\",\n        \"Accelerated filer\",\n        \"Non-accelerated filer\",\n        \"Smaller reporting company\"\n      ]\n    }\n  },\n  \"required\": [\"cik\", \"name\"],\n  \"$defs\": {\n    \"Address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"street1\": {\n          \"type\": \"string\"\n        },\n        \"street2\": {\n          \"type\": \"string\"\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"stateOrCountry\": {\n          \"\
  type\": \"string\"\n        },\n        \"zipCode\": {\n          \"type\": \"string\"\n        },\n        \"stateOrCountryDescription\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sec-edgar/refs/heads/main/json-schema/sec-edgar-company-schema.json
tags: []
title: SEC EDGAR Company
---
