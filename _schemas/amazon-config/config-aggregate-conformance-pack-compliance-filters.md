---
description: Filters the conformance packs based on an account ID, region, compliance type, and the name of the conformance pack.
layout: schema
name: AggregateConformancePackComplianceFilters
properties_list:
- description: ''
  name: ConformancePackName
  type: object
- description: ''
  name: ComplianceType
  type: object
- description: ''
  name: AccountId
  type: object
- description: ''
  name: AwsRegion
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-aggregate-conformance-pack-compliance-filters-schema.json
slug: config-aggregate-conformance-pack-compliance-filters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-aggregate-conformance-pack-compliance-filters-schema.json\",\n  \"title\": \"AggregateConformancePackComplianceFilters\",\n  \"description\": \"Filters the conformance packs based on an account ID, region, compliance type, and the name of the conformance pack.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConformancePackName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackName\"\n        },\n        {\n          \"description\": \"The name of the conformance pack.\"\n        }\n      ]\n    },\n    \"ComplianceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackComplianceType\"\n        },\n        {\n          \"description\": \"The compliance status of the conformance pack.\"\n        }\n   \
  \   ]\n    },\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The 12-digit Amazon Web Services account ID of the source account.\"\n        }\n      ]\n    },\n    \"AwsRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsRegion\"\n        },\n        {\n          \"description\": \"The source Amazon Web Services Region from where the data is aggregated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-aggregate-conformance-pack-compliance-filters-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: AggregateConformancePackComplianceFilters
---
