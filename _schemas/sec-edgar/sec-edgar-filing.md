---
description: An SEC EDGAR filing submission record including metadata and document index
layout: schema
name: SEC EDGAR Filing
properties_list:
- description: Unique accession number in XXXXXXXXXX-YY-ZZZZZZ format
  name: accessionNumber
  type: string
- description: Central Index Key (10-digit with leading zeros)
  name: cik
  type: string
- description: Registrant entity name
  name: entityName
  type: string
- description: SEC form type
  name: formType
  type: string
- description: Date the filing was accepted by EDGAR
  name: filingDate
  type: string
- description: Period of report end date
  name: reportDate
  type: string
- description: Exact date-time of acceptance by EDGAR
  name: acceptanceDateTime
  type: string
- description: Securities Act under which filed
  name: act
  type: string
- description: SEC file number for the registrant
  name: fileNumber
  type: string
- description: Film number assigned to the filing
  name: filmNumber
  type: string
- description: Form 8-K item numbers (comma-separated)
  name: items
  type: string
- description: Total filing size in bytes
  name: size
  type: integer
- description: Whether filing includes XBRL data
  name: isXBRL
  type: boolean
- description: Whether filing uses Inline XBRL (iXBRL)
  name: isInlineXBRL
  type: boolean
- description: Filename of the primary filing document
  name: primaryDocument
  type: string
- description: Description of the primary document
  name: primaryDocDescription
  type: string
- description: All documents included in the filing
  name: documents
  type: array
- description: ''
  name: xbrlData
  type: object
provider_name: sec-edgar
provider_slug: sec-edgar
schema_file: json-schema/sec-edgar-filing-schema.json
slug: sec-edgar-filing
source_filename: sec-edgar-filing-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://data.sec.gov/schemas/filing\",\n  \"title\": \"SEC EDGAR Filing\",\n  \"description\": \"An SEC EDGAR filing submission record including metadata and document index\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessionNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Unique accession number in XXXXXXXXXX-YY-ZZZZZZ format\",\n      \"pattern\": \"^\\\\d{10}-\\\\d{2}-\\\\d{6}$\",\n      \"examples\": [\"0000320193-23-000106\"]\n    },\n    \"cik\": {\n      \"type\": \"string\",\n      \"description\": \"Central Index Key (10-digit with leading zeros)\",\n      \"pattern\": \"^\\\\d{10}$\",\n      \"examples\": [\"0000320193\"]\n    },\n    \"entityName\": {\n      \"type\": \"string\",\n      \"description\": \"Registrant entity name\",\n      \"examples\": [\"Apple Inc.\"]\n    },\n    \"formType\": {\n      \"type\": \"string\",\n      \"description\": \"\
  SEC form type\",\n      \"examples\": [\"10-K\", \"10-Q\", \"8-K\", \"DEF 14A\", \"S-1\", \"4\", \"SC 13G\"]\n    },\n    \"filingDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the filing was accepted by EDGAR\"\n    },\n    \"reportDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Period of report end date\"\n    },\n    \"acceptanceDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Exact date-time of acceptance by EDGAR\"\n    },\n    \"act\": {\n      \"type\": \"string\",\n      \"description\": \"Securities Act under which filed\",\n      \"examples\": [\"34\", \"33\"]\n    },\n    \"fileNumber\": {\n      \"type\": \"string\",\n      \"description\": \"SEC file number for the registrant\"\n    },\n    \"filmNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Film number assigned to the filing\"\n    },\n    \"items\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Form 8-K item numbers (comma-separated)\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"Total filing size in bytes\"\n    },\n    \"isXBRL\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether filing includes XBRL data\"\n    },\n    \"isInlineXBRL\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether filing uses Inline XBRL (iXBRL)\"\n    },\n    \"primaryDocument\": {\n      \"type\": \"string\",\n      \"description\": \"Filename of the primary filing document\"\n    },\n    \"primaryDocDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the primary document\"\n    },\n    \"documents\": {\n      \"type\": \"array\",\n      \"description\": \"All documents included in the filing\",\n      \"items\": {\n        \"$ref\": \"#/$defs/FilingDocument\"\n      }\n    },\n    \"xbrlData\": {\n      \"$ref\": \"#/$defs/XBRLSummary\"\n    }\n\
  \  },\n  \"required\": [\"accessionNumber\", \"cik\", \"formType\", \"filingDate\"],\n  \"$defs\": {\n    \"FilingDocument\": {\n      \"type\": \"object\",\n      \"description\": \"A single document within a filing submission\",\n      \"properties\": {\n        \"sequence\": {\n          \"type\": \"integer\",\n          \"description\": \"Document sequence number\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Document description\"\n        },\n        \"documentName\": {\n          \"type\": \"string\",\n          \"description\": \"Filename of the document\"\n        },\n        \"documentType\": {\n          \"type\": \"string\",\n          \"description\": \"SEC document type code\"\n        },\n        \"size\": {\n          \"type\": \"integer\",\n          \"description\": \"Document size in bytes\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\"\
  : \"Full URL to document on EDGAR\"\n        }\n      },\n      \"required\": [\"documentName\", \"documentType\"]\n    },\n    \"XBRLSummary\": {\n      \"type\": \"object\",\n      \"description\": \"Summary of XBRL financial data in the filing\",\n      \"properties\": {\n        \"taxonomy\": {\n          \"type\": \"string\",\n          \"enum\": [\"us-gaap\", \"ifrs-full\", \"dei\"],\n          \"description\": \"Primary XBRL taxonomy used\"\n        },\n        \"concepts\": {\n          \"type\": \"array\",\n          \"description\": \"XBRL concept names reported\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"periodOfReport\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"End date of reporting period\"\n        },\n        \"fiscalYear\": {\n          \"type\": \"integer\",\n          \"description\": \"Fiscal year\"\n        },\n        \"fiscalPeriod\": {\n          \"type\"\
  : \"string\",\n          \"enum\": [\"FY\", \"Q1\", \"Q2\", \"Q3\", \"Q4\"],\n          \"description\": \"Fiscal period\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sec-edgar/refs/heads/main/json-schema/sec-edgar-filing-schema.json
tags: []
title: SEC EDGAR Filing
---
