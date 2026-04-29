---
description: A banded (alternating colors) range in a sheet.
layout: schema
name: BandedRange
properties_list:
- description: The ID of the banded range.
  name: bandedRangeId
  type: integer
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-banded-range-schema.json
slug: google-sheets-banded-range
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BandedRange\",\n  \"type\": \"object\",\n  \"description\": \"A banded (alternating colors) range in a sheet.\",\n  \"properties\": {\n    \"bandedRangeId\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the banded range.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-banded-range-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: BandedRange
---
