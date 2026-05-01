---
description: FilterCriteriaMap schema from AWS IAM Access Analyzer API
layout: schema
name: FilterCriteriaMap
properties_list: []
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-filter-criteria-map-schema.json
slug: iam-access-analyzer-filter-criteria-map
source_filename: iam-access-analyzer-filter-criteria-map-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-filter-criteria-map-schema.json\",\n  \"title\": \"FilterCriteriaMap\",\n  \"description\": \"FilterCriteriaMap schema from AWS IAM Access Analyzer API\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"eq\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ValueList\"\n          },\n          {\n            \"description\": \"An \\\"equals\\\" operator to match for the filter used to create the rule.\"\n          }\n        ]\n      },\n      \"neq\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ValueList\"\n          },\n          {\n            \"description\": \"A \\\"not equals\\\" operator to match for the filter used to create the\
  \ rule.\"\n          }\n        ]\n      },\n      \"contains\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ValueList\"\n          },\n          {\n            \"description\": \"A \\\"contains\\\" operator to match for the filter used to create the rule.\"\n          }\n        ]\n      },\n      \"exists\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Boolean\"\n          },\n          {\n            \"description\": \"An \\\"exists\\\" operator to match for the filter used to create the rule. \"\n          }\n        ]\n      }\n    },\n    \"description\": \"The criteria to use in the filter that defines the archive rule. For more information on available filter keys, see <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/access-analyzer-reference-filter-keys.html\\\">IAM Access Analyzer filter keys</a>.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-filter-criteria-map-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: FilterCriteriaMap
---
