---
description: UpdateLedgerPermissionsModeResponse schema from Amazon QLDB API
layout: schema
name: UpdateLedgerPermissionsModeResponse
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: PermissionsMode
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-update-ledger-permissions-mode-response-schema.json
slug: amazon-qldb-update-ledger-permissions-mode-response
source_filename: amazon-qldb-update-ledger-permissions-mode-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-update-ledger-permissions-mode-response-schema.json\",\n  \"title\": \"UpdateLedgerPermissionsModeResponse\",\n  \"description\": \"UpdateLedgerPermissionsModeResponse schema from Amazon QLDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LedgerName\"\n        },\n        {\n          \"description\": \"The name of the ledger.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the ledger.\"\n        }\n      ]\n    },\n    \"PermissionsMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionsMode\"\n\
  \        },\n        {\n          \"description\": \"The current permissions mode of the ledger.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-update-ledger-permissions-mode-response-schema.json
tags:
- AWS
- Blockchain
- Database
- Ledger
title: UpdateLedgerPermissionsModeResponse
---
