---
description: A compliance score is the percentage of the number of compliant rule-resource combinations in a conformance pack compared to the number of total possible rule-resource combinations in the conformance pack. This metric provides you with a high-level view of the compliance state of your conformance packs. You can use it to identify, investigate, and understand the level of compliance in your conformance packs.
layout: schema
name: ConformancePackComplianceScore
properties_list:
- description: ''
  name: Score
  type: object
- description: ''
  name: ConformancePackName
  type: object
- description: ''
  name: LastUpdatedTime
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-conformance-pack-compliance-score-schema.json
slug: config-conformance-pack-compliance-score
source_filename: config-conformance-pack-compliance-score-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-conformance-pack-compliance-score-schema.json\",\n  \"title\": \"ConformancePackComplianceScore\",\n  \"description\": \"A compliance score is the percentage of the number of compliant rule-resource combinations in a conformance pack compared to the number of total possible rule-resource combinations in the conformance pack. This metric provides you with a high-level view of the compliance state of your conformance packs. You can use it to identify, investigate, and understand the level of compliance in your conformance packs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Score\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComplianceScore\"\n        },\n        {\n          \"description\": \"Compliance score for the conformance pack. Conformance packs with\
  \ no evaluation results will have a compliance score of <code>INSUFFICIENT_DATA</code>.\"\n        }\n      ]\n    },\n    \"ConformancePackName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackName\"\n        },\n        {\n          \"description\": \"The name of the conformance pack.\"\n        }\n      ]\n    },\n    \"LastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdatedTime\"\n        },\n        {\n          \"description\": \"The time that the conformance pack compliance score was last updated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-conformance-pack-compliance-score-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: ConformancePackComplianceScore
---
