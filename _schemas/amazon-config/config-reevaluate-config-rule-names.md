---
description: ReevaluateConfigRuleNames schema
layout: schema
name: ReevaluateConfigRuleNames
properties_list: []
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-reevaluate-config-rule-names-schema.json
slug: config-reevaluate-config-rule-names
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-reevaluate-config-rule-names-schema.json\",\n  \"title\": \"ReevaluateConfigRuleNames\",\n  \"description\": \"ReevaluateConfigRuleNames schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/ConfigRuleName\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 25\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-reevaluate-config-rule-names-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ReevaluateConfigRuleNames
---
