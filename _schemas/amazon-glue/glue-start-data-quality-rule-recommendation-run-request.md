---
description: StartDataQualityRuleRecommendationRunRequest schema from Amazon Glue API
layout: schema
name: StartDataQualityRuleRecommendationRunRequest
properties_list:
- description: ''
  name: DataSource
  type: object
- description: ''
  name: Role
  type: object
- description: ''
  name: NumberOfWorkers
  type: object
- description: ''
  name: Timeout
  type: object
- description: ''
  name: CreatedRulesetName
  type: object
- description: ''
  name: ClientToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-start-data-quality-rule-recommendation-run-request-schema.json
slug: glue-start-data-quality-rule-recommendation-run-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-start-data-quality-rule-recommendation-run-request-schema.json\",\n  \"title\": \"StartDataQualityRuleRecommendationRunRequest\",\n  \"description\": \"StartDataQualityRuleRecommendationRunRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DataSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSource\"\n        },\n        {\n          \"description\": \"The data source (Glue table) associated with this run.\"\n        }\n      ]\n    },\n    \"Role\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleString\"\n        },\n        {\n          \"description\": \"An IAM role supplied to encrypt the results of the run.\"\n        }\n      ]\n    },\n    \"NumberOfWorkers\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"The number of <code>G.1X</code> workers to be used in the run. The default is 5.\"\n        }\n      ]\n    },\n    \"Timeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timeout\"\n        },\n        {\n          \"description\": \"The timeout for a run in minutes. This is the maximum time that a run can consume resources before it is terminated and enters <code>TIMEOUT</code> status. The default is 2,880 minutes (48 hours).\"\n        }\n      ]\n    },\n    \"CreatedRulesetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"A name for the ruleset.\"\n        }\n      ]\n    },\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"\
  description\": \"Used for idempotency and is recommended to be set to a random ID (such as a UUID) to avoid creating or starting multiple instances of the same resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DataSource\",\n    \"Role\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-start-data-quality-rule-recommendation-run-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: StartDataQualityRuleRecommendationRunRequest
---
