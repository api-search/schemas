---
description: Summary count of items in an import deployment, showing total, imported, failed, and skipped counts.
layout: schema
name: ImportSummaryCount
properties_list:
- description: Total number of items in the package.
  name: total
  type: integer
- description: Number of items successfully imported.
  name: imported
  type: integer
- description: Number of items that failed to import.
  name: failed
  type: integer
- description: Number of items skipped during import.
  name: skipped
  type: integer
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-import-summary-count-schema.json
slug: deployment-rest-import-summary-count
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-import-summary-count-schema.json\",\n  \"title\": \"ImportSummaryCount\",\n  \"description\": \"Summary count of items in an import deployment, showing total, imported, failed, and skipped counts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of items in the package.\",\n      \"minimum\": 0\n    },\n    \"imported\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of items successfully imported.\",\n      \"minimum\": 0\n    },\n    \"failed\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of items that failed to import.\",\n      \"minimum\": 0\n    },\n    \"skipped\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of items skipped during import.\",\n\
  \      \"minimum\": 0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-import-summary-count-schema.json
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: ImportSummaryCount
---
