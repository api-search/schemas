---
description: Full structural metadata of a Crystal Report
layout: schema
name: ReportStructure
properties_list:
- description: Data sources used by the report
  name: datasources
  type: array
- description: Fields used in the report
  name: usedfields
  type: array
- description: Group conditions defined in the report
  name: groupconditions
  type: array
- description: Report parameters
  name: parameters
  type: array
- description: Summary fields in the report
  name: summary
  type: array
- description: Running total fields
  name: runningtotals
  type: array
- description: Formula fields defined in the report
  name: formulas
  type: array
- description: Subreports embedded in the report
  name: subreports
  type: array
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-report-structure-schema.json
slug: crystal-reports-report-structure
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-report-structure-schema.json\",\n  \"title\": \"ReportStructure\",\n  \"description\": \"Full structural metadata of a Crystal Report\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"datasources\": {\n      \"type\": \"array\",\n      \"description\": \"Data sources used by the report\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DataSource\"\n      }\n    },\n    \"usedfields\": {\n      \"type\": \"array\",\n      \"description\": \"Fields used in the report\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UsedField\"\n      }\n    },\n    \"groupconditions\": {\n      \"type\": \"array\",\n      \"description\": \"Group conditions defined in the report\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/GroupCondition\"\n      }\n\
  \    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"Report parameters\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ReportParameter\"\n      }\n    },\n    \"summary\": {\n      \"type\": \"array\",\n      \"description\": \"Summary fields in the report\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SummaryField\"\n      }\n    },\n    \"runningtotals\": {\n      \"type\": \"array\",\n      \"description\": \"Running total fields\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/RunningTotal\"\n      }\n    },\n    \"formulas\": {\n      \"type\": \"array\",\n      \"description\": \"Formula fields defined in the report\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Formula\"\n      }\n    },\n    \"subreports\": {\n      \"type\": \"array\",\n      \"description\": \"Subreports embedded in the report\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Subreport\"\n     \
  \ }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-report-structure-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: ReportStructure
---
