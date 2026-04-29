---
description: ListDataQualityRulesetEvaluationRunsResponse schema from Amazon Glue API
layout: schema
name: ListDataQualityRulesetEvaluationRunsResponse
properties_list:
- description: ''
  name: Runs
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-list-data-quality-ruleset-evaluation-runs-response-schema.json
slug: glue-list-data-quality-ruleset-evaluation-runs-response
source_filename: glue-list-data-quality-ruleset-evaluation-runs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-data-quality-ruleset-evaluation-runs-response-schema.json\",\n  \"title\": \"ListDataQualityRulesetEvaluationRunsResponse\",\n  \"description\": \"ListDataQualityRulesetEvaluationRunsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Runs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataQualityRulesetEvaluationRunList\"\n        },\n        {\n          \"description\": \"A list of <code>DataQualityRulesetEvaluationRunDescription</code> objects representing data quality ruleset runs.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"A pagination token, if more results are available.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-data-quality-ruleset-evaluation-runs-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: ListDataQualityRulesetEvaluationRunsResponse
---
