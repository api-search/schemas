---
description: A protected range.
layout: schema
name: ProtectedRange
properties_list:
- description: The ID of the protected range.
  name: protectedRangeId
  type: integer
- description: The named range this protected range is backed by, if any.
  name: namedRangeId
  type: string
- description: The description of this protected range.
  name: description
  type: string
- description: True if this protected range will show a warning when editing.
  name: warningOnly
  type: boolean
- description: True if the user who requested this protected range can edit the protected area.
  name: requestingUserCanEdit
  type: boolean
- description: The list of unprotected ranges within a protected sheet.
  name: unprotectedRanges
  type: array
- description: The users and groups with edit access to the protected range.
  name: editors
  type: object
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-protected-range-schema.json
slug: google-sheets-protected-range
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProtectedRange\",\n  \"type\": \"object\",\n  \"description\": \"A protected range.\",\n  \"properties\": {\n    \"protectedRangeId\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the protected range.\"\n    },\n    \"namedRangeId\": {\n      \"type\": \"string\",\n      \"description\": \"The named range this protected range is backed by, if any.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of this protected range.\"\n    },\n    \"warningOnly\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if this protected range will show a warning when editing.\"\n    },\n    \"requestingUserCanEdit\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the user who requested this protected range can edit the protected area.\"\n    },\n    \"unprotectedRanges\": {\n      \"type\": \"array\"\
  ,\n      \"description\": \"The list of unprotected ranges within a protected sheet.\"\n    },\n    \"editors\": {\n      \"type\": \"object\",\n      \"description\": \"The users and groups with edit access to the protected range.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-protected-range-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: ProtectedRange
---
