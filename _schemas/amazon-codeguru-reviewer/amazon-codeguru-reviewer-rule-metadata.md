---
description: Metadata about a rule. Rule metadata includes an ID, a name, a list of tags, and a short and long description. CodeGuru Reviewer uses rules to analyze code. A rule's recommendation is included in analysis results if code is detected that violates the rule.
layout: schema
name: RuleMetadata
properties_list:
- description: ''
  name: RuleId
  type: object
- description: ''
  name: RuleName
  type: object
- description: ''
  name: ShortDescription
  type: object
- description: ''
  name: LongDescription
  type: object
- description: ''
  name: RuleTags
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-rule-metadata-schema.json
slug: amazon-codeguru-reviewer-rule-metadata
source_filename: amazon-codeguru-reviewer-rule-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-rule-metadata-schema.json\",\n  \"title\": \"RuleMetadata\",\n  \"description\": \"Metadata about a rule. Rule metadata includes an ID, a name, a list of tags, and a short and long description. CodeGuru Reviewer uses rules to analyze code. A rule's recommendation is included in analysis results if code is detected that violates the rule.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleId\"\n        },\n        {\n          \"description\": \"The ID of the rule.\"\n        }\n      ]\n    },\n    \"RuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleName\"\n        },\n        {\n          \"description\": \"The name of the rule.\"\n\
  \        }\n      ]\n    },\n    \"ShortDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShortDescription\"\n        },\n        {\n          \"description\": \"A short description of the rule.\"\n        }\n      ]\n    },\n    \"LongDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongDescription\"\n        },\n        {\n          \"description\": \"A long description of the rule.\"\n        }\n      ]\n    },\n    \"RuleTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleTags\"\n        },\n        {\n          \"description\": \"Tags that are associated with the rule.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-rule-metadata-schema.json
tags:
- Amazon
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: RuleMetadata
---
