---
description: CreateFindingsReportRequest schema
layout: schema
name: CreateFindingsReportRequest
properties_list:
- description: ''
  name: filterCriteria
  type: object
- description: ''
  name: reportFormat
  type: object
- description: ''
  name: s3Destination
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-create-findings-report-request-schema.json
slug: inspector-create-findings-report-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-create-findings-report-request-schema.json\",\n  \"title\": \"CreateFindingsReportRequest\",\n  \"description\": \"CreateFindingsReportRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filterCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterCriteria\"\n        },\n        {\n          \"description\": \"The filter criteria to apply to the results of the finding report.\"\n        }\n      ]\n    },\n    \"reportFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportFormat\"\n        },\n        {\n          \"description\": \"The format to generate the report in.\"\n        }\n      ]\n    },\n    \"s3Destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Destination\"\
  \n        },\n        {\n          \"description\": \"The Amazon S3 export destination for the report.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"reportFormat\",\n    \"s3Destination\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-create-findings-report-request-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: CreateFindingsReportRequest
---
