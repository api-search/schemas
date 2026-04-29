---
description: Schema defining the structure of an Amazon Athena query execution resource, including query string, execution context, result configuration, work group settings, and execution status.
layout: schema
name: Amazon Athena Query Execution
properties_list:
- description: The unique identifier for each query execution.
  name: QueryExecutionId
  type: string
- description: The SQL query statements which the query execution ran.
  name: QueryString
  type: string
- description: The type of query statement that was run.
  name: StatementType
  type: string
- description: ''
  name: ResultConfiguration
  type: object
- description: ''
  name: QueryExecutionContext
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: Statistics
  type: object
- description: The name of the workgroup in which the query ran.
  name: WorkGroup
  type: string
- description: ''
  name: EngineVersion
  type: object
- description: A list of values for the parameters in a query.
  name: ExecutionParameters
  type: array
- description: The kind of query statement that was run.
  name: SubstatementType
  type: string
provider_name: Amazon Athena
provider_slug: amazon-athena
schema_file: json-schema/amazon-athena-schema.json
slug: amazon-athena
source_filename: amazon-athena-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.apievangelist.com/amazon-athena/query-execution\",\n  \"title\": \"Amazon Athena Query Execution\",\n  \"description\": \"Schema defining the structure of an Amazon Athena query execution resource, including query string, execution context, result configuration, work group settings, and execution status.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"QueryString\"\n  ],\n  \"properties\": {\n    \"QueryExecutionId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for each query execution.\"\n    },\n    \"QueryString\": {\n      \"type\": \"string\",\n      \"description\": \"The SQL query statements which the query execution ran.\",\n      \"minLength\": 1,\n      \"maxLength\": 262144\n    },\n    \"StatementType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"DDL\",\n        \"DML\",\n        \"UTILITY\"\n      ],\n    \
  \  \"description\": \"The type of query statement that was run.\"\n    },\n    \"ResultConfiguration\": {\n      \"$ref\": \"#/$defs/ResultConfiguration\"\n    },\n    \"QueryExecutionContext\": {\n      \"$ref\": \"#/$defs/QueryExecutionContext\"\n    },\n    \"Status\": {\n      \"$ref\": \"#/$defs/QueryExecutionStatus\"\n    },\n    \"Statistics\": {\n      \"$ref\": \"#/$defs/QueryExecutionStatistics\"\n    },\n    \"WorkGroup\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the workgroup in which the query ran.\"\n    },\n    \"EngineVersion\": {\n      \"$ref\": \"#/$defs/EngineVersion\"\n    },\n    \"ExecutionParameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A list of values for the parameters in a query.\"\n    },\n    \"SubstatementType\": {\n      \"type\": \"string\",\n      \"description\": \"The kind of query statement that was run.\"\n    }\n  },\n  \"$defs\": {\n    \"\
  ResultConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"The location in Amazon S3 where query results are stored and the encryption option, if any, used for query results.\",\n      \"properties\": {\n        \"OutputLocation\": {\n          \"type\": \"string\",\n          \"description\": \"The location in Amazon S3 where your query results are stored.\"\n        },\n        \"EncryptionConfiguration\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"EncryptionOption\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"SSE_S3\",\n                \"SSE_KMS\",\n                \"CSE_KMS\"\n              ],\n              \"description\": \"The type of server-side encryption used.\"\n            },\n            \"KmsKey\": {\n              \"type\": \"string\",\n              \"description\": \"The KMS key ARN or ID for SSE_KMS and CSE_KMS encryption.\"\n            }\n          },\n          \"required\"\
  : [\n            \"EncryptionOption\"\n          ]\n        },\n        \"ExpectedBucketOwner\": {\n          \"type\": \"string\",\n          \"description\": \"The Amazon Web Services account ID that you expect to be the owner of the Amazon S3 bucket.\"\n        },\n        \"AclConfiguration\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"S3AclOption\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"BUCKET_OWNER_FULL_CONTROL\"\n              ]\n            }\n          }\n        }\n      }\n    },\n    \"QueryExecutionContext\": {\n      \"type\": \"object\",\n      \"description\": \"The database and data catalog context for the query execution.\",\n      \"properties\": {\n        \"Database\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the database used in the query execution.\"\n        },\n        \"Catalog\": {\n          \"type\": \"string\",\n          \"description\":\
  \ \"The name of the data catalog used in the query execution.\"\n        }\n      }\n    },\n    \"QueryExecutionStatus\": {\n      \"type\": \"object\",\n      \"description\": \"The status of a query execution.\",\n      \"properties\": {\n        \"State\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"QUEUED\",\n            \"RUNNING\",\n            \"SUCCEEDED\",\n            \"FAILED\",\n            \"CANCELLED\"\n          ],\n          \"description\": \"The state of the query execution.\"\n        },\n        \"StateChangeReason\": {\n          \"type\": \"string\",\n          \"description\": \"Further detail about the status of the query.\"\n        },\n        \"SubmissionDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time that the query was submitted.\"\n        },\n        \"CompletionDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\
  ,\n          \"description\": \"The date and time that the query completed.\"\n        },\n        \"AthenaError\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"ErrorCategory\": {\n              \"type\": \"integer\"\n            },\n            \"ErrorType\": {\n              \"type\": \"integer\"\n            },\n            \"Retryable\": {\n              \"type\": \"boolean\"\n            },\n            \"ErrorMessage\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"QueryExecutionStatistics\": {\n      \"type\": \"object\",\n      \"description\": \"Statistics about the query execution.\",\n      \"properties\": {\n        \"EngineExecutionTimeInMillis\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of milliseconds that the query took to execute.\"\n        },\n        \"DataScannedInBytes\": {\n          \"type\": \"integer\",\n          \"description\": \"The\
  \ number of bytes in the data that was queried.\"\n        },\n        \"DataManifestLocation\": {\n          \"type\": \"string\",\n          \"description\": \"The location and file name of a data manifest file.\"\n        },\n        \"TotalExecutionTimeInMillis\": {\n          \"type\": \"integer\"\n        },\n        \"QueryQueueTimeInMillis\": {\n          \"type\": \"integer\"\n        },\n        \"ServicePreProcessingTimeInMillis\": {\n          \"type\": \"integer\"\n        },\n        \"ServiceProcessingTimeInMillis\": {\n          \"type\": \"integer\"\n        },\n        \"ResultReuseInformation\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"ReusedPreviousResult\": {\n              \"type\": \"boolean\"\n            }\n          }\n        }\n      }\n    },\n    \"EngineVersion\": {\n      \"type\": \"object\",\n      \"description\": \"The Athena engine version for running queries.\",\n      \"properties\": {\n        \"SelectedEngineVersion\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The engine version requested by the user.\"\n        },\n        \"EffectiveEngineVersion\": {\n          \"type\": \"string\",\n          \"description\": \"The engine version that ran the query.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-athena/refs/heads/main/json-schema/amazon-athena-schema.json
tags:
- Amazon Athena
- SQL
- Analytics
- Serverless
- AWS
title: Amazon Athena Query Execution
---
