---
description: PeopleSoft GL journal entry.
layout: schema
name: JournalEntry
properties_list:
- description: Business unit.
  name: BUSINESS_UNIT
  type: string
- description: Journal ID.
  name: JOURNAL_ID
  type: string
- description: Journal date.
  name: JOURNAL_DATE
  type: string
- description: Ledger name.
  name: LEDGER
  type: string
- description: Journal description.
  name: DESCR
  type: string
- description: Journal status.
  name: JRNL_HDR_STATUS
  type: string
- description: Currency code.
  name: CURRENCY_CD
  type: string
- description: Fiscal year.
  name: FISCAL_YEAR
  type: integer
- description: Accounting period.
  name: ACCOUNTING_PERIOD
  type: integer
- description: Journal lines.
  name: LINES
  type: array
provider_name: PeopleSoft
provider_slug: peoplesoft
schema_file: json-schema/peoplesoft-financials-journal-entry-schema.json
slug: peoplesoft-financials-journal-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/json-schema/peoplesoft-financials-journal-entry-schema.json\",\n  \"title\": \"JournalEntry\",\n  \"description\": \"PeopleSoft GL journal entry.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BUSINESS_UNIT\": {\n      \"type\": \"string\",\n      \"description\": \"Business unit.\",\n      \"example\": \"US001\"\n    },\n    \"JOURNAL_ID\": {\n      \"type\": \"string\",\n      \"description\": \"Journal ID.\",\n      \"example\": \"0000012345\"\n    },\n    \"JOURNAL_DATE\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Journal date.\",\n      \"example\": \"2026-04-17\"\n    },\n    \"LEDGER\": {\n      \"type\": \"string\",\n      \"description\": \"Ledger name.\",\n      \"example\": \"ACTUALS\"\n    },\n    \"DESCR\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Journal description.\",\n      \"example\": \"Monthly accrual entry\"\n    },\n    \"JRNL_HDR_STATUS\": {\n      \"type\": \"string\",\n      \"description\": \"Journal status.\",\n      \"enum\": [\n        \"N\",\n        \"E\",\n        \"V\",\n        \"P\",\n        \"D\",\n        \"U\",\n        \"T\"\n      ],\n      \"example\": \"V\"\n    },\n    \"CURRENCY_CD\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code.\",\n      \"example\": \"USD\"\n    },\n    \"FISCAL_YEAR\": {\n      \"type\": \"integer\",\n      \"description\": \"Fiscal year.\",\n      \"example\": 2026\n    },\n    \"ACCOUNTING_PERIOD\": {\n      \"type\": \"integer\",\n      \"description\": \"Accounting period.\",\n      \"example\": 4\n    },\n    \"LINES\": {\n      \"type\": \"array\",\n      \"description\": \"Journal lines.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"JOURNAL_LINE\": {\n            \"type\": \"integer\",\n     \
  \       \"description\": \"Line number.\",\n            \"example\": 1\n          },\n          \"ACCOUNT\": {\n            \"type\": \"string\",\n            \"description\": \"GL account.\",\n            \"example\": \"510000\"\n          },\n          \"DEPTID\": {\n            \"type\": \"string\",\n            \"description\": \"Department.\",\n            \"example\": \"10200\"\n          },\n          \"MONETARY_AMOUNT\": {\n            \"type\": \"number\",\n            \"description\": \"Amount.\",\n            \"example\": 5000.0\n          },\n          \"LINE_DESCR\": {\n            \"type\": \"string\",\n            \"description\": \"Line description.\",\n            \"example\": \"Office supplies\"\n          }\n        }\n      }\n    }\n  },\n  \"x-schema-source\": \"domain-knowledge\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/json-schema/peoplesoft-financials-journal-entry-schema.json
tags:
- Campus Solutions
- CRM
- Enterprise Software
- ERP
- Financial Management
- HCM
- Supply Chain Management
title: JournalEntry
---
