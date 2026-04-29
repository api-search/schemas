---
description: Result of an import deployment operation, including a summary of imported, failed, and skipped objects, Admin Console settings, plug-ins, and database scripts.
layout: schema
name: ImportDeploymentResult
properties_list:
- description: ''
  name: status
  type: object
- description: Summary of the import deployment operation results.
  name: summary
  type: object
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-import-deployment-result-schema.json
slug: deployment-rest-import-deployment-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-import-deployment-result-schema.json\",\n  \"title\": \"ImportDeploymentResult\",\n  \"description\": \"Result of an import deployment operation, including a summary of imported, failed, and skipped objects, Admin Console settings, plug-ins, and database scripts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"$ref\": \"#/components/schemas/DeploymentStatus\"\n    },\n    \"summary\": {\n      \"type\": \"object\",\n      \"description\": \"Summary of the import deployment operation results.\",\n      \"properties\": {\n        \"objects\": {\n          \"$ref\": \"#/components/schemas/ImportSummaryCount\"\n        },\n        \"adminConsoleSettings\": {\n          \"$ref\": \"#/components/schemas/ImportSummaryCount\"\n        },\n        \"plugins\": {\n          \"\
  type\": \"object\",\n          \"description\": \"Summary of plug-in import results.\",\n          \"properties\": {\n            \"total\": {\n              \"type\": \"integer\",\n              \"description\": \"Total number of plug-ins in the package.\",\n              \"minimum\": 0\n            },\n            \"imported\": {\n              \"type\": \"integer\",\n              \"description\": \"Number of plug-ins successfully imported.\",\n              \"minimum\": 0\n            },\n            \"skipped\": {\n              \"type\": \"integer\",\n              \"description\": \"Number of plug-ins skipped during import.\",\n              \"minimum\": 0\n            }\n          }\n        },\n        \"databaseScripts\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of database scripts executed during import.\",\n          \"minimum\": 0\n        },\n        \"deploymentLogUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n\
  \          \"description\": \"URL to retrieve the full deployment log.\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"summary\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-import-deployment-result-schema.json
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: ImportDeploymentResult
---
