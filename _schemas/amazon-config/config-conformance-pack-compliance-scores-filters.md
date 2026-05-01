---
description: A list of filters to apply to the conformance pack compliance score result set.
layout: schema
name: ConformancePackComplianceScoresFilters
properties_list:
- description: ''
  name: ConformancePackNames
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-conformance-pack-compliance-scores-filters-schema.json
slug: config-conformance-pack-compliance-scores-filters
source_filename: config-conformance-pack-compliance-scores-filters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-conformance-pack-compliance-scores-filters-schema.json\",\n  \"title\": \"ConformancePackComplianceScoresFilters\",\n  \"description\": \"A list of filters to apply to the conformance pack compliance score result set. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConformancePackNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackNameFilter\"\n        },\n        {\n          \"description\": \"The names of the conformance packs whose compliance scores you want to include in the conformance pack compliance score result set. You can include up to 25 conformance packs in the <code>ConformancePackNames</code> array of strings, each with a character limit of 256 characters for the conformance pack name.\"\n        }\n      ]\n    }\n  },\n  \"\
  required\": [\n    \"ConformancePackNames\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-conformance-pack-compliance-scores-filters-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: ConformancePackComplianceScoresFilters
---
