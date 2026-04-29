---
description: Information about a ledger, including its name, state, and when it was created.
layout: schema
name: LedgerSummary
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: CreationDateTime
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-ledger-summary-schema.json
slug: amazon-qldb-ledger-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-ledger-summary-schema.json\",\n  \"title\": \"LedgerSummary\",\n  \"description\": \"Information about a ledger, including its name, state, and when it was created.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LedgerName\"\n        },\n        {\n          \"description\": \"The name of the ledger.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LedgerState\"\n        },\n        {\n          \"description\": \"The current status of the ledger.\"\n        }\n      ]\n    },\n    \"CreationDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\"\
  : \"The date and time, in epoch time format, when the ledger was created. (Epoch time format is the number of seconds elapsed since 12:00:00 AM January 1, 1970 UTC.)\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-ledger-summary-schema.json
tags:
- AWS
- Blockchain
- Database
- Ledger
title: LedgerSummary
---
