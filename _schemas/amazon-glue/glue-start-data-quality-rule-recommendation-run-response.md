---
description: StartDataQualityRuleRecommendationRunResponse schema from Amazon Glue API
layout: schema
name: StartDataQualityRuleRecommendationRunResponse
properties_list:
- description: ''
  name: RunId
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-start-data-quality-rule-recommendation-run-response-schema.json
slug: glue-start-data-quality-rule-recommendation-run-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-start-data-quality-rule-recommendation-run-response-schema.json\",\n  \"title\": \"StartDataQualityRuleRecommendationRunResponse\",\n  \"description\": \"StartDataQualityRuleRecommendationRunResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RunId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"The unique run identifier associated with this run.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-start-data-quality-rule-recommendation-run-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: StartDataQualityRuleRecommendationRunResponse
---
