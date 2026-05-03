---
description: A journal entry records financial transactions in the general ledger, consisting of balanced debit and credit lines posted to specific ledger accounts within a Workday Financial Management system.
layout: schema
name: Workday Journal Entry
properties_list:
- description: Workday ID (WID) uniquely identifying the journal entry
  name: id
  type: string
- description: System-generated journal entry number
  name: journalNumber
  type: string
- description: Date of the journal entry
  name: journalDate
  type: string
- description: Descriptive memo for the journal entry
  name: description
  type: string
- description: Current lifecycle status of the journal entry
  name: status
  type: string
- description: Source system or process that created the journal entry
  name: journalSource
  type: string
- description: Company entity associated with the journal entry
  name: company
  type: object
- description: Transaction currency
  name: currency
  type: object
- description: Accounting period for the journal entry
  name: accountingPeriod
  type: object
- description: Total debit amount across all lines
  name: totalDebit
  type: number
- description: Total credit amount across all lines
  name: totalCredit
  type: number
- description: Individual journal entry lines (minimum two required for balanced entry)
  name: lines
  type: array
- description: Worker who created the journal entry
  name: createdBy
  type: object
- description: Timestamp when the journal entry was created
  name: createdOn
  type: string
provider_name: Workday Financials
provider_slug: workday-financials
schema_file: json-schema/workday-financials-journal-entry-schema.json
slug: workday-financials-journal-entry
source_filename: workday-financials-journal-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://community.workday.com/schemas/workday-financials/journal-entry.json\",\n  \"title\": \"Workday Journal Entry\",\n  \"description\": \"A journal entry records financial transactions in the general ledger, consisting of balanced debit and credit lines posted to specific ledger accounts within a Workday Financial Management system.\",\n  \"type\": \"object\",\n  \"required\": [\"journalDate\", \"company\", \"lines\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Workday ID (WID) uniquely identifying the journal entry\"\n    },\n    \"journalNumber\": {\n      \"type\": \"string\",\n      \"description\": \"System-generated journal entry number\"\n    },\n    \"journalDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of the journal entry\"\n    },\n    \"description\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Descriptive memo for the journal entry\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Draft\", \"Submitted\", \"Approved\", \"Posted\", \"Reversed\"],\n      \"description\": \"Current lifecycle status of the journal entry\"\n    },\n    \"journalSource\": {\n      \"type\": \"string\",\n      \"description\": \"Source system or process that created the journal entry\"\n    },\n    \"company\": {\n      \"$ref\": \"#/$defs/Reference\",\n      \"description\": \"Company entity associated with the journal entry\"\n    },\n    \"currency\": {\n      \"$ref\": \"#/$defs/Reference\",\n      \"description\": \"Transaction currency\"\n    },\n    \"accountingPeriod\": {\n      \"$ref\": \"#/$defs/Reference\",\n      \"description\": \"Accounting period for the journal entry\"\n    },\n    \"totalDebit\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Total debit amount across all lines\"\n    },\n    \"\
  totalCredit\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Total credit amount across all lines\"\n    },\n    \"lines\": {\n      \"type\": \"array\",\n      \"minItems\": 2,\n      \"items\": {\n        \"$ref\": \"#/$defs/JournalLine\"\n      },\n      \"description\": \"Individual journal entry lines (minimum two required for balanced entry)\"\n    },\n    \"createdBy\": {\n      \"$ref\": \"#/$defs/Reference\",\n      \"description\": \"Worker who created the journal entry\"\n    },\n    \"createdOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the journal entry was created\"\n    }\n  },\n  \"$defs\": {\n    \"JournalLine\": {\n      \"type\": \"object\",\n      \"description\": \"An individual line within a journal entry representing a debit or credit to a ledger account\",\n      \"properties\": {\n        \"ledgerAccount\": {\n          \"$ref\": \"#/$defs/Reference\",\n        \
  \  \"description\": \"Ledger account for this line\"\n        },\n        \"debitAmount\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"description\": \"Debit amount for this line\"\n        },\n        \"creditAmount\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"description\": \"Credit amount for this line\"\n        },\n        \"memo\": {\n          \"type\": \"string\",\n          \"description\": \"Line-level memo\"\n        },\n        \"costCenter\": {\n          \"$ref\": \"#/$defs/Reference\",\n          \"description\": \"Cost center allocation for this line\"\n        }\n      }\n    },\n    \"Reference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a related Workday resource\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Workday ID (WID) of the referenced resource\"\n        },\n        \"descriptor\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"Display name of the referenced resource\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday-financials/refs/heads/main/json-schema/workday-financials-journal-entry-schema.json
tags:
- Accounting
- Cloud ERP
- Financial Management
- Procurement
title: Workday Journal Entry
---
