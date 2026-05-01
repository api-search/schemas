---
description: GetConformancePackComplianceDetailsRequest schema
layout: schema
name: GetConformancePackComplianceDetailsRequest
properties_list:
- description: ''
  name: ConformancePackName
  type: object
- description: ''
  name: Filters
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-conformance-pack-compliance-details-request-schema.json
slug: config-get-conformance-pack-compliance-details-request
source_filename: config-get-conformance-pack-compliance-details-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-conformance-pack-compliance-details-request-schema.json\",\n  \"title\": \"GetConformancePackComplianceDetailsRequest\",\n  \"description\": \"GetConformancePackComplianceDetailsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConformancePackName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackName\"\n        },\n        {\n          \"description\": \"Name of the conformance pack.\"\n        }\n      ]\n    },\n    \"Filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackEvaluationFilters\"\n        },\n        {\n          \"description\": \"A <code>ConformancePackEvaluationFilters</code> object.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/GetConformancePackComplianceDetailsLimit\"\n        },\n        {\n          \"description\": \"The maximum number of evaluation results returned on each page. If you do no specify a number, Config uses the default. The default is 100.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned in a previous request that you use to request the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConformancePackName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-conformance-pack-compliance-details-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: GetConformancePackComplianceDetailsRequest
---
