---
description: ListDataQualityRulesetsResponse schema from Amazon Glue API
layout: schema
name: ListDataQualityRulesetsResponse
properties_list:
- description: ''
  name: Rulesets
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-list-data-quality-rulesets-response-schema.json
slug: glue-list-data-quality-rulesets-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-data-quality-rulesets-response-schema.json\",\n  \"title\": \"ListDataQualityRulesetsResponse\",\n  \"description\": \"ListDataQualityRulesetsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Rulesets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataQualityRulesetList\"\n        },\n        {\n          \"description\": \"A paginated list of rulesets for the specified list of Glue tables.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"A pagination token, if more results are available.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-data-quality-rulesets-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: ListDataQualityRulesetsResponse
---
