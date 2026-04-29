---
description: ListConformancePackComplianceScoresResponse schema
layout: schema
name: ListConformancePackComplianceScoresResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: ConformancePackComplianceScores
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-list-conformance-pack-compliance-scores-response-schema.json
slug: config-list-conformance-pack-compliance-scores-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-list-conformance-pack-compliance-scores-response-schema.json\",\n  \"title\": \"ListConformancePackComplianceScoresResponse\",\n  \"description\": \"ListConformancePackComplianceScoresResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string that you can use to get the next page of results in a paginated response.\"\n        }\n      ]\n    },\n    \"ConformancePackComplianceScores\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackComplianceScores\"\n        },\n        {\n          \"description\": \"A list of <code>ConformancePackComplianceScore</code>\
  \ objects.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConformancePackComplianceScores\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-list-conformance-pack-compliance-scores-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ListConformancePackComplianceScoresResponse
---
