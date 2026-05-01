---
description: GetFindingsReportStatusResponse schema
layout: schema
name: GetFindingsReportStatusResponse
properties_list:
- description: ''
  name: destination
  type: object
- description: ''
  name: errorCode
  type: object
- description: ''
  name: errorMessage
  type: object
- description: ''
  name: filterCriteria
  type: object
- description: ''
  name: reportId
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-get-findings-report-status-response-schema.json
slug: inspector-get-findings-report-status-response
source_filename: inspector-get-findings-report-status-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-get-findings-report-status-response-schema.json\",\n  \"title\": \"GetFindingsReportStatusResponse\",\n  \"description\": \"GetFindingsReportStatusResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Destination\"\n        },\n        {\n          \"description\": \"The destination of the report.\"\n        }\n      ]\n    },\n    \"errorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportingErrorCode\"\n        },\n        {\n          \"description\": \"The error code of the report.\"\n        }\n      ]\n    },\n    \"errorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorMessage\"\n        },\n   \
  \     {\n          \"description\": \"The error message of the report.\"\n        }\n      ]\n    },\n    \"filterCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterCriteria\"\n        },\n        {\n          \"description\": \"The filter criteria associated with the report.\"\n        }\n      ]\n    },\n    \"reportId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportId\"\n        },\n        {\n          \"description\": \"The ID of the report.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalReportStatus\"\n        },\n        {\n          \"description\": \"The status of the report.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-get-findings-report-status-response-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: GetFindingsReportStatusResponse
---
