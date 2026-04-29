---
description: ListDataQualityRulesetEvaluationRunsRequest schema from Amazon Glue API
layout: schema
name: ListDataQualityRulesetEvaluationRunsRequest
properties_list:
- description: ''
  name: Filter
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-list-data-quality-ruleset-evaluation-runs-request-schema.json
slug: glue-list-data-quality-ruleset-evaluation-runs-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-data-quality-ruleset-evaluation-runs-request-schema.json\",\n  \"title\": \"ListDataQualityRulesetEvaluationRunsRequest\",\n  \"description\": \"ListDataQualityRulesetEvaluationRunsRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Filter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataQualityRulesetEvaluationRunFilter\"\n        },\n        {\n          \"description\": \"The filter criteria.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"A paginated token to offset the results.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n        \
  \  \"$ref\": \"#/components/schemas/PageSize\"\n        },\n        {\n          \"description\": \"The maximum number of results to return.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-data-quality-ruleset-evaluation-runs-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: ListDataQualityRulesetEvaluationRunsRequest
---
