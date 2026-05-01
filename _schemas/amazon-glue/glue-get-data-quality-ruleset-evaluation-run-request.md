---
description: GetDataQualityRulesetEvaluationRunRequest schema from Amazon Glue API
layout: schema
name: GetDataQualityRulesetEvaluationRunRequest
properties_list:
- description: ''
  name: RunId
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-data-quality-ruleset-evaluation-run-request-schema.json
slug: glue-get-data-quality-ruleset-evaluation-run-request
source_filename: glue-get-data-quality-ruleset-evaluation-run-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-data-quality-ruleset-evaluation-run-request-schema.json\",\n  \"title\": \"GetDataQualityRulesetEvaluationRunRequest\",\n  \"description\": \"GetDataQualityRulesetEvaluationRunRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RunId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"The unique run identifier associated with this run.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RunId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-data-quality-ruleset-evaluation-run-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetDataQualityRulesetEvaluationRunRequest
---
