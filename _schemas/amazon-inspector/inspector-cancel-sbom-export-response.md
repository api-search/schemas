---
description: CancelSbomExportResponse schema
layout: schema
name: CancelSbomExportResponse
properties_list:
- description: ''
  name: reportId
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-cancel-sbom-export-response-schema.json
slug: inspector-cancel-sbom-export-response
source_filename: inspector-cancel-sbom-export-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-cancel-sbom-export-response-schema.json\",\n  \"title\": \"CancelSbomExportResponse\",\n  \"description\": \"CancelSbomExportResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reportId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportId\"\n        },\n        {\n          \"description\": \"The report ID of the canceled SBOM export.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-cancel-sbom-export-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: CancelSbomExportResponse
---
