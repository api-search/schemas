---
description: Returns a filtered list of Detective or Proactive Config rules. By default, if the filter is not defined, this API returns an unfiltered list. For more information on Detective or Proactive Config rules, see <a href="https://docs.aws.amazon.com/config/latest/developerguide/evaluate-config-rules.html"> <b>Evaluation Mode</b> </a> in the <i>Config Developer Guide</i>.
layout: schema
name: DescribeConfigRulesFilters
properties_list:
- description: ''
  name: EvaluationMode
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-config-rules-filters-schema.json
slug: config-describe-config-rules-filters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-config-rules-filters-schema.json\",\n  \"title\": \"DescribeConfigRulesFilters\",\n  \"description\": \"Returns a filtered list of Detective or Proactive Config rules. By default, if the filter is not defined, this API returns an unfiltered list. For more information on Detective or Proactive Config rules, see <a href=\\\"https://docs.aws.amazon.com/config/latest/developerguide/evaluate-config-rules.html\\\"> <b>Evaluation Mode</b> </a> in the <i>Config Developer Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EvaluationMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EvaluationMode\"\n        },\n        {\n          \"description\": \"The mode of an evaluation. The valid values are Detective or Proactive.\"\n        }\n      ]\n   \
  \ }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-config-rules-filters-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeConfigRulesFilters
---
