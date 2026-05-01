---
description: CancelFindingsReportRequest schema
layout: schema
name: CancelFindingsReportRequest
properties_list:
- description: ''
  name: reportId
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-cancel-findings-report-request-schema.json
slug: inspector-cancel-findings-report-request
source_filename: inspector-cancel-findings-report-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-cancel-findings-report-request-schema.json\",\n  \"title\": \"CancelFindingsReportRequest\",\n  \"description\": \"CancelFindingsReportRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reportId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportId\"\n        },\n        {\n          \"description\": \"The ID of the report to be canceled.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"reportId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-cancel-findings-report-request-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: CancelFindingsReportRequest
---
