---
description: Collection of errors and warnings identified during a package inspection.
layout: schema
name: InspectionProblems
properties_list:
- description: Total number of errors found during inspection.
  name: totalErrors
  type: integer
- description: Total number of warnings found during inspection.
  name: totalWarnings
  type: integer
- description: Array of error details identified during inspection.
  name: errors
  type: array
- description: Array of warning details identified during inspection.
  name: warnings
  type: array
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-inspection-problems-schema.json
slug: deployment-rest-inspection-problems
source_filename: deployment-rest-inspection-problems-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-inspection-problems-schema.json\",\n  \"title\": \"InspectionProblems\",\n  \"description\": \"Collection of errors and warnings identified during a package inspection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalErrors\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of errors found during inspection.\",\n      \"minimum\": 0\n    },\n    \"totalWarnings\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of warnings found during inspection.\",\n      \"minimum\": 0\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"Array of error details identified during inspection.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/InspectionError\"\n      }\n    },\n    \"warnings\": {\n      \"type\"\
  : \"array\",\n      \"description\": \"Array of warning details identified during inspection.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/InspectionWarning\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-inspection-problems-schema.json
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: InspectionProblems
---
