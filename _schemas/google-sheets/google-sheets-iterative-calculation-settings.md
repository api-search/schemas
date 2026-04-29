---
description: Settings to control how circular dependencies are resolved with iterative calculation.
layout: schema
name: IterativeCalculationSettings
properties_list:
- description: When iterative calculation is enabled, the maximum number of calculation rounds to perform.
  name: maxIterations
  type: integer
- description: When iterative calculation is enabled and successive results differ by less than this threshold value, the calculation rounds stop.
  name: convergenceThreshold
  type: number
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-iterative-calculation-settings-schema.json
slug: google-sheets-iterative-calculation-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IterativeCalculationSettings\",\n  \"type\": \"object\",\n  \"description\": \"Settings to control how circular dependencies are resolved with iterative calculation.\",\n  \"properties\": {\n    \"maxIterations\": {\n      \"type\": \"integer\",\n      \"description\": \"When iterative calculation is enabled, the maximum number of calculation rounds to perform.\"\n    },\n    \"convergenceThreshold\": {\n      \"type\": \"number\",\n      \"description\": \"When iterative calculation is enabled and successive results differ by less than this threshold value, the calculation rounds stop.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-iterative-calculation-settings-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: IterativeCalculationSettings
---
