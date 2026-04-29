---
description: GetDataQualityRulesetResponse schema from Amazon Glue API
layout: schema
name: GetDataQualityRulesetResponse
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Ruleset
  type: object
- description: ''
  name: TargetTable
  type: object
- description: ''
  name: CreatedOn
  type: object
- description: ''
  name: LastModifiedOn
  type: object
- description: ''
  name: RecommendationRunId
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-data-quality-ruleset-response-schema.json
slug: glue-get-data-quality-ruleset-response
source_filename: glue-get-data-quality-ruleset-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-data-quality-ruleset-response-schema.json\",\n  \"title\": \"GetDataQualityRulesetResponse\",\n  \"description\": \"GetDataQualityRulesetResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the ruleset.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescriptionString\"\n        },\n        {\n          \"description\": \"A description of the ruleset.\"\n        }\n      ]\n    },\n    \"Ruleset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataQualityRulesetString\"\n        },\n    \
  \    {\n          \"description\": \"A Data Quality Definition Language (DQDL) ruleset. For more information, see the Glue developer guide.\"\n        }\n      ]\n    },\n    \"TargetTable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataQualityTargetTable\"\n        },\n        {\n          \"description\": \"The name and database name of the target table.\"\n        }\n      ]\n    },\n    \"CreatedOn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A timestamp. The time and date that this data quality ruleset was created.\"\n        }\n      ]\n    },\n    \"LastModifiedOn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A timestamp. The last point in time when this data quality ruleset was modified.\"\n        }\n      ]\n    },\n    \"RecommendationRunId\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"When a ruleset was created from a recommendation run, this run ID is generated to link the two together.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-data-quality-ruleset-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetDataQualityRulesetResponse
---
