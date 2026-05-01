---
description: These are custom parameters to be used when the target is a Amazon Redshift cluster to invoke the Amazon Redshift Data API ExecuteStatement.
layout: schema
name: PipeTargetRedshiftDataParameters
properties_list:
- description: ''
  name: Database
  type: object
- description: ''
  name: DbUser
  type: object
- description: ''
  name: SecretManagerArn
  type: object
- description: ''
  name: Sqls
  type: object
- description: ''
  name: StatementName
  type: object
- description: ''
  name: WithEvent
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-pipe-target-redshift-data-parameters-schema.json
slug: amazon-eventbridge-pipes-pipe-target-redshift-data-parameters
source_filename: amazon-eventbridge-pipes-pipe-target-redshift-data-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-redshift-data-parameters-schema.json\",\n  \"title\": \"PipeTargetRedshiftDataParameters\",\n  \"description\": \"These are custom parameters to be used when the target is a Amazon Redshift cluster to invoke the Amazon Redshift Data API ExecuteStatement.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Database\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Database\"\n        },\n        {\n          \"description\": \"The name of the database. Required when authenticating using temporary credentials.\"\n        }\n      ]\n    },\n    \"DbUser\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DbUser\"\n        },\n        {\n          \"description\": \"The database user name. Required\
  \ when authenticating using temporary credentials.\"\n        }\n      ]\n    },\n    \"SecretManagerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecretManagerArnOrJsonPath\"\n        },\n        {\n          \"description\": \"The name or ARN of the secret that enables access to the database. Required when authenticating using SageMaker.\"\n        }\n      ]\n    },\n    \"Sqls\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Sqls\"\n        },\n        {\n          \"description\": \"The SQL statement text to run.\"\n        }\n      ]\n    },\n    \"StatementName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatementName\"\n        },\n        {\n          \"description\": \"The name of the SQL statement. You can name the SQL statement when you create it to identify the query.\"\n        }\n      ]\n    },\n    \"WithEvent\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Indicates whether to send an event back to EventBridge after the SQL statement runs.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Database\",\n    \"Sqls\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-redshift-data-parameters-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: PipeTargetRedshiftDataParameters
---
