---
description: The number of conformance packs that are compliant and noncompliant.
layout: schema
name: AggregateConformancePackComplianceCount
properties_list:
- description: ''
  name: CompliantConformancePackCount
  type: object
- description: ''
  name: NonCompliantConformancePackCount
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-aggregate-conformance-pack-compliance-count-schema.json
slug: config-aggregate-conformance-pack-compliance-count
source_filename: config-aggregate-conformance-pack-compliance-count-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-aggregate-conformance-pack-compliance-count-schema.json\",\n  \"title\": \"AggregateConformancePackComplianceCount\",\n  \"description\": \"The number of conformance packs that are compliant and noncompliant.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CompliantConformancePackCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Number of compliant conformance packs.\"\n        }\n      ]\n    },\n    \"NonCompliantConformancePackCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Number of noncompliant conformance packs.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-aggregate-conformance-pack-compliance-count-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: AggregateConformancePackComplianceCount
---
