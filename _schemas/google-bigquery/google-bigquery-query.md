---
description: Schema for a BigQuery query request, used to execute SQL queries against BigQuery datasets.
layout: schema
name: Google BigQuery Query Request
properties_list:
- description: A query string to execute, using GoogleSQL or legacy SQL syntax
  name: query
  type: string
- description: The maximum number of rows of data to return per page of results
  name: maxResults
  type: integer
- description: The default dataset to use for unqualified table names in the query
  name: defaultDataset
  type: object
- description: Whether to use legacy SQL dialect. If false, uses GoogleSQL.
  name: useLegacySql
  type: boolean
- description: How long to wait for the query to complete, in milliseconds
  name: timeoutMs
  type: integer
- description: If set to true, BigQuery does not run the job but instead returns statistics about the job
  name: dryRun
  type: boolean
- description: Whether to look for the result in the query cache
  name: useQueryCache
  type: boolean
- description: Standard SQL only. Set to POSITIONAL to use positional query parameters or NAMED for named parameters.
  name: parameterMode
  type: string
- description: Query parameters for GoogleSQL queries
  name: queryParameters
  type: array
provider_name: Google BigQuery
provider_slug: google-bigquery
schema_file: json-schema/google-bigquery-query-schema.json
slug: google-bigquery-query
source_filename: google-bigquery-query-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://cloud.google.com/schemas/bigquery/query.json\",\n  \"title\": \"Google BigQuery Query Request\",\n  \"description\": \"Schema for a BigQuery query request, used to execute SQL queries against BigQuery datasets.\",\n  \"type\": \"object\",\n  \"required\": [\"query\"],\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"A query string to execute, using GoogleSQL or legacy SQL syntax\",\n      \"minLength\": 1\n    },\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of rows of data to return per page of results\",\n      \"minimum\": 0\n    },\n    \"defaultDataset\": {\n      \"$ref\": \"#/$defs/DatasetReference\",\n      \"description\": \"The default dataset to use for unqualified table names in the query\"\n    },\n    \"useLegacySql\": {\n      \"type\": \"boolean\",\n      \"description\": \"\
  Whether to use legacy SQL dialect. If false, uses GoogleSQL.\",\n      \"default\": false\n    },\n    \"timeoutMs\": {\n      \"type\": \"integer\",\n      \"description\": \"How long to wait for the query to complete, in milliseconds\",\n      \"minimum\": 0\n    },\n    \"dryRun\": {\n      \"type\": \"boolean\",\n      \"description\": \"If set to true, BigQuery does not run the job but instead returns statistics about the job\",\n      \"default\": false\n    },\n    \"useQueryCache\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to look for the result in the query cache\",\n      \"default\": true\n    },\n    \"parameterMode\": {\n      \"type\": \"string\",\n      \"description\": \"Standard SQL only. Set to POSITIONAL to use positional query parameters or NAMED for named parameters.\",\n      \"enum\": [\"POSITIONAL\", \"NAMED\"]\n    },\n    \"queryParameters\": {\n      \"type\": \"array\",\n      \"description\": \"Query parameters for GoogleSQL queries\"\
  ,\n      \"items\": {\n        \"$ref\": \"#/$defs/QueryParameter\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"DatasetReference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a BigQuery dataset\",\n      \"properties\": {\n        \"projectId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the project containing the dataset\"\n        },\n        \"datasetId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the dataset\"\n        }\n      }\n    },\n    \"QueryParameter\": {\n      \"type\": \"object\",\n      \"description\": \"A query parameter for parameterized queries\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of this parameter. Used for named parameters only.\"\n        },\n        \"parameterType\": {\n          \"type\": \"object\",\n          \"description\": \"The type of this parameter\",\n          \"properties\"\
  : {\n            \"type\": {\n              \"type\": \"string\",\n              \"description\": \"The data type\",\n              \"enum\": [\"STRING\", \"INT64\", \"FLOAT64\", \"NUMERIC\", \"BIGNUMERIC\", \"BOOL\", \"BYTES\", \"DATE\", \"DATETIME\", \"GEOGRAPHY\", \"TIME\", \"TIMESTAMP\", \"ARRAY\", \"STRUCT\"]\n            }\n          }\n        },\n        \"parameterValue\": {\n          \"type\": \"object\",\n          \"description\": \"The value of this parameter\",\n          \"properties\": {\n            \"value\": {\n              \"type\": \"string\",\n              \"description\": \"The value of this parameter\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-bigquery/refs/heads/main/json-schema/google-bigquery-query-schema.json
tags:
- Analytics
- Big Data
- Cloud
- Data Warehouse
- Serverless
- SQL
title: Google BigQuery Query Request
---
