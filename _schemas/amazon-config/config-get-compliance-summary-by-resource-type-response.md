---
description: <p/>
layout: schema
name: GetComplianceSummaryByResourceTypeResponse
properties_list:
- description: ''
  name: ComplianceSummariesByResourceType
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-compliance-summary-by-resource-type-response-schema.json
slug: config-get-compliance-summary-by-resource-type-response
source_filename: config-get-compliance-summary-by-resource-type-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-compliance-summary-by-resource-type-response-schema.json\",\n  \"title\": \"GetComplianceSummaryByResourceTypeResponse\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ComplianceSummariesByResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComplianceSummariesByResourceType\"\n        },\n        {\n          \"description\": \"The number of resources that are compliant and the number that are noncompliant. If one or more resource types were provided with the request, the numbers are returned for each resource type. The maximum number returned is 100.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-compliance-summary-by-resource-type-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: GetComplianceSummaryByResourceTypeResponse
---
