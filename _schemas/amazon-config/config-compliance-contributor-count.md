---
description: The number of Amazon Web Services resources or Config rules responsible for the current compliance of the item, up to a maximum number.
layout: schema
name: ComplianceContributorCount
properties_list:
- description: ''
  name: CappedCount
  type: object
- description: ''
  name: CapExceeded
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-compliance-contributor-count-schema.json
slug: config-compliance-contributor-count
source_filename: config-compliance-contributor-count-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-compliance-contributor-count-schema.json\",\n  \"title\": \"ComplianceContributorCount\",\n  \"description\": \"The number of Amazon Web Services resources or Config rules responsible for the current compliance of the item, up to a maximum number.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CappedCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of Amazon Web Services resources or Config rules responsible for the current compliance of the item.\"\n        }\n      ]\n    },\n    \"CapExceeded\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Indicates whether the maximum count is reached.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-compliance-contributor-count-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ComplianceContributorCount
---
