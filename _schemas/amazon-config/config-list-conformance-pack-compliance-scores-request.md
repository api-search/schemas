---
description: ListConformancePackComplianceScoresRequest schema
layout: schema
name: ListConformancePackComplianceScoresRequest
properties_list:
- description: ''
  name: Filters
  type: object
- description: ''
  name: SortOrder
  type: object
- description: ''
  name: SortBy
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-list-conformance-pack-compliance-scores-request-schema.json
slug: config-list-conformance-pack-compliance-scores-request
source_filename: config-list-conformance-pack-compliance-scores-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-list-conformance-pack-compliance-scores-request-schema.json\",\n  \"title\": \"ListConformancePackComplianceScoresRequest\",\n  \"description\": \"ListConformancePackComplianceScoresRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackComplianceScoresFilters\"\n        },\n        {\n          \"description\": \"Filters the results based on the <code>ConformancePackComplianceScoresFilters</code>.\"\n        }\n      ]\n    },\n    \"SortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrder\"\n        },\n        {\n          \"description\": \"<p>Determines the order in which conformance pack compliance scores are sorted. Either in ascending\
  \ or descending order.</p> <p>By default, conformance pack compliance scores are sorted in alphabetical order by name of the conformance pack. Conformance pack compliance scores are sorted in reverse alphabetical order if you enter <code>DESCENDING</code>.</p> <p>You can sort conformance pack compliance scores by the numerical value of the compliance score by entering <code>SCORE</code> in the <code>SortBy</code> action. When compliance scores are sorted by <code>SCORE</code>, conformance packs with a compliance score of <code>INSUFFICIENT_DATA</code> will be last when sorting by ascending order and first when sorting by descending order.</p>\"\n        }\n      ]\n    },\n    \"SortBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortBy\"\n        },\n        {\n          \"description\": \"<p>Sorts your conformance pack compliance scores in either ascending or descending order, depending on <code>SortOrder</code>.</p> <p>By default, conformance pack\
  \ compliance scores are sorted in alphabetical order by name of the conformance pack. Enter <code>SCORE</code>, to sort conformance pack compliance scores by the numerical value of the compliance score.</p>\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageSizeLimit\"\n        },\n        {\n          \"description\": \"The maximum number of conformance pack compliance scores returned on each page.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string in a prior request that you can use to get the paginated response for the next set of conformance pack compliance scores.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-list-conformance-pack-compliance-scores-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ListConformancePackComplianceScoresRequest
---
