---
description: GetDataQualityRulesetEvaluationRunResponse schema from Amazon Glue API
layout: schema
name: GetDataQualityRulesetEvaluationRunResponse
properties_list:
- description: ''
  name: RunId
  type: object
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
  name: AdditionalRunOptions
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: ErrorString
  type: object
- description: ''
  name: StartedOn
  type: object
- description: ''
  name: LastModifiedOn
  type: object
- description: ''
  name: CompletedOn
  type: object
- description: ''
  name: ExecutionTime
  type: object
- description: ''
  name: RulesetNames
  type: object
- description: ''
  name: ResultIds
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-data-quality-ruleset-evaluation-run-response-schema.json
slug: glue-get-data-quality-ruleset-evaluation-run-response
source_filename: glue-get-data-quality-ruleset-evaluation-run-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-data-quality-ruleset-evaluation-run-response-schema.json\",\n  \"title\": \"GetDataQualityRulesetEvaluationRunResponse\",\n  \"description\": \"GetDataQualityRulesetEvaluationRunResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RunId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"The unique run identifier associated with this run.\"\n        }\n      ]\n    },\n    \"DataSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSource\"\n        },\n        {\n          \"description\": \"The data source (an Glue table) associated with this evaluation run.\"\n        }\n      ]\n    },\n    \"Role\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/RoleString\"\n        },\n        {\n          \"description\": \"An IAM role supplied to encrypt the results of the run.\"\n        }\n      ]\n    },\n    \"NumberOfWorkers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"The number of <code>G.1X</code> workers to be used in the run. The default is 5.\"\n        }\n      ]\n    },\n    \"Timeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timeout\"\n        },\n        {\n          \"description\": \"The timeout for a run in minutes. This is the maximum time that a run can consume resources before it is terminated and enters <code>TIMEOUT</code> status. The default is 2,880 minutes (48 hours).\"\n        }\n      ]\n    },\n    \"AdditionalRunOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataQualityEvaluationRunAdditionalRunOptions\"\
  \n        },\n        {\n          \"description\": \"Additional run options you can specify for an evaluation run.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskStatusType\"\n        },\n        {\n          \"description\": \"The status for this run.\"\n        }\n      ]\n    },\n    \"ErrorString\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The error strings that are associated with the run.\"\n        }\n      ]\n    },\n    \"StartedOn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when this run started.\"\n        }\n      ]\n    },\n    \"LastModifiedOn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\"\
  : \"A timestamp. The last point in time when this data quality rule recommendation run was modified.\"\n        }\n      ]\n    },\n    \"CompletedOn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when this run was completed.\"\n        }\n      ]\n    },\n    \"ExecutionTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionTime\"\n        },\n        {\n          \"description\": \"The amount of time (in seconds) that the run consumed resources.\"\n        }\n      ]\n    },\n    \"RulesetNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RulesetNames\"\n        },\n        {\n          \"description\": \"A list of ruleset names for the run.\"\n        }\n      ]\n    },\n    \"ResultIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataQualityResultIdList\"\n   \
  \     },\n        {\n          \"description\": \"A list of result IDs for the data quality results for the run.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-data-quality-ruleset-evaluation-run-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetDataQualityRulesetEvaluationRunResponse
---
