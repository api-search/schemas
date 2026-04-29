---
description: An object containing <code>RuleName</code>, and <code>MatchingKeys</code>.
layout: schema
name: Rule
properties_list:
- description: ''
  name: matchingKeys
  type: object
- description: ''
  name: ruleName
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-rule-schema.json
slug: amazon-entity-resolution-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-rule-schema.json\",\n  \"title\": \"Rule\",\n  \"description\": \"An object containing <code>RuleName</code>, and <code>MatchingKeys</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"matchingKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleMatchingKeysList\"\n        },\n        {\n          \"description\": \"A list of <code>MatchingKeys</code>. The <code>MatchingKeys</code> must have been defined in the <code>SchemaMapping</code>. Two records are considered to match according to this rule if all of the <code>MatchingKeys</code> match.\"\n        }\n      ]\n    },\n    \"ruleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleRuleNameString\"\n        },\n        {\n          \"\
  description\": \"A name for the matching rule.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"matchingKeys\",\n    \"ruleName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-rule-schema.json
tags:
- Amazon Web Services
- AWS
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: Rule
---
