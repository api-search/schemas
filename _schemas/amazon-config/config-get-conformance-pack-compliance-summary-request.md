---
description: GetConformancePackComplianceSummaryRequest schema
layout: schema
name: GetConformancePackComplianceSummaryRequest
properties_list:
- description: ''
  name: ConformancePackNames
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-conformance-pack-compliance-summary-request-schema.json
slug: config-get-conformance-pack-compliance-summary-request
source_filename: config-get-conformance-pack-compliance-summary-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-conformance-pack-compliance-summary-request-schema.json\",\n  \"title\": \"GetConformancePackComplianceSummaryRequest\",\n  \"description\": \"GetConformancePackComplianceSummaryRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConformancePackNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackNamesToSummarizeList\"\n        },\n        {\n          \"description\": \"Names of conformance packs.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageSizeLimit\"\n        },\n        {\n          \"description\": \"The maximum number of conformance packs returned on each page.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The nextToken string returned on a previous page that you use to get the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConformancePackNames\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-conformance-pack-compliance-summary-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: GetConformancePackComplianceSummaryRequest
---
