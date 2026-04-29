---
description: Result of a package inspection operation, including expected object counts and any problems identified.
layout: schema
name: InspectionResult
properties_list:
- description: The current status of the inspection operation.
  name: status
  type: string
- description: Summary of the inspection findings.
  name: summary
  type: object
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-inspection-result-schema.json
slug: deployment-rest-inspection-result
source_filename: deployment-rest-inspection-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-inspection-result-schema.json\",\n  \"title\": \"InspectionResult\",\n  \"description\": \"Result of a package inspection operation, including expected object counts and any problems identified.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the inspection operation.\",\n      \"enum\": [\n        \"IN_PROGRESS\",\n        \"COMPLETED\",\n        \"FAILED\"\n      ]\n    },\n    \"summary\": {\n      \"type\": \"object\",\n      \"description\": \"Summary of the inspection findings.\",\n      \"properties\": {\n        \"objectsExpected\": {\n          \"$ref\": \"#/components/schemas/ImportSummaryCount\"\n        },\n        \"adminConsoleSettingsExpected\": {\n          \"$ref\": \"#/components/schemas/ImportSummaryCount\"\
  \n        },\n        \"problems\": {\n          \"$ref\": \"#/components/schemas/InspectionProblems\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-inspection-result-schema.json
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: InspectionResult
---
