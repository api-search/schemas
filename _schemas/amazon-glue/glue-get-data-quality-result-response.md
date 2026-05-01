---
description: GetDataQualityResultResponse schema from Amazon Glue API
layout: schema
name: GetDataQualityResultResponse
properties_list:
- description: ''
  name: ResultId
  type: object
- description: ''
  name: Score
  type: object
- description: ''
  name: DataSource
  type: object
- description: ''
  name: RulesetName
  type: object
- description: ''
  name: EvaluationContext
  type: object
- description: ''
  name: StartedOn
  type: object
- description: ''
  name: CompletedOn
  type: object
- description: ''
  name: JobName
  type: object
- description: ''
  name: JobRunId
  type: object
- description: ''
  name: RulesetEvaluationRunId
  type: object
- description: ''
  name: RuleResults
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-data-quality-result-response-schema.json
slug: glue-get-data-quality-result-response
source_filename: glue-get-data-quality-result-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-data-quality-result-response-schema.json\",\n  \"title\": \"GetDataQualityResultResponse\",\n  \"description\": \"GetDataQualityResultResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResultId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"A unique result ID for the data quality result.\"\n        }\n      ]\n    },\n    \"Score\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericBoundedDouble\"\n        },\n        {\n          \"description\": \"An aggregate data quality score. Represents the ratio of rules that passed to the total number of rules.\"\n        }\n      ]\n    },\n    \"DataSource\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/DataSource\"\n        },\n        {\n          \"description\": \"The table associated with the data quality result, if any.\"\n        }\n      ]\n    },\n    \"RulesetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the ruleset associated with the data quality result.\"\n        }\n      ]\n    },\n    \"EvaluationContext\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"In the context of a job in Glue Studio, each node in the canvas is typically assigned some sort of name and data quality nodes will have names. In the case of multiple nodes, the <code>evaluationContext</code> can differentiate the nodes.\"\n        }\n      ]\n    },\n    \"StartedOn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\
  \n        },\n        {\n          \"description\": \"The date and time when the run for this data quality result started.\"\n        }\n      ]\n    },\n    \"CompletedOn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the run for this data quality result was completed.\"\n        }\n      ]\n    },\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The job name associated with the data quality result, if any.\"\n        }\n      ]\n    },\n    \"JobRunId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"The job run ID associated with the data quality result, if any.\"\n        }\n      ]\n    },\n    \"RulesetEvaluationRunId\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"The unique run ID associated with the ruleset evaluation.\"\n        }\n      ]\n    },\n    \"RuleResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataQualityRuleResults\"\n        },\n        {\n          \"description\": \"A list of <code>DataQualityRuleResult</code> objects representing the results for each rule. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-data-quality-result-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetDataQualityResultResponse
---
