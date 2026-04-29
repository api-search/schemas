---
description: <p/>
layout: schema
name: DescribeConfigRulesRequest
properties_list:
- description: ''
  name: ConfigRuleNames
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Filters
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-config-rules-request-schema.json
slug: config-describe-config-rules-request
source_filename: config-describe-config-rules-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-config-rules-request-schema.json\",\n  \"title\": \"DescribeConfigRulesRequest\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRuleNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigRuleNames\"\n        },\n        {\n          \"description\": \"The names of the Config rules for which you want details. If you do not specify any names, Config returns details for all your rules.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response.\"\n        }\n\
  \      ]\n    },\n    \"Filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescribeConfigRulesFilters\"\n        },\n        {\n          \"description\": \"Returns a list of Detective or Proactive Config rules. By default, this API returns an unfiltered list. For more information on Detective or Proactive Config rules, see <a href=\\\"https://docs.aws.amazon.com/config/latest/developerguide/evaluate-config-rules.html\\\"> <b>Evaluation Mode</b> </a> in the <i>Config Developer Guide</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-config-rules-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeConfigRulesRequest
---
