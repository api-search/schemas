---
description: CancelFindingsReportResponse schema
layout: schema
name: CancelFindingsReportResponse
properties_list:
- description: ''
  name: reportId
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-cancel-findings-report-response-schema.json
slug: inspector-cancel-findings-report-response
source_filename: inspector-cancel-findings-report-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-cancel-findings-report-response-schema.json\",\n  \"title\": \"CancelFindingsReportResponse\",\n  \"description\": \"CancelFindingsReportResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reportId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportId\"\n        },\n        {\n          \"description\": \"The ID of the canceled report.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"reportId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-cancel-findings-report-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: CancelFindingsReportResponse
---
